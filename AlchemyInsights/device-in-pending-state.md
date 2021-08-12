---
title: Laite odottavassa tilassa
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: 224e6e613c306b50e354930bcbe6f43f1c08528766cb6e681b0e9826b2d55a4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914000"
---
# <a name="device-in-pending-state"></a>Laite odottavassa tilassa

**Edellytykset:**

1. Jos määrität laiterekisteröintiä ensimmäistä kertaa, varmista, että olet tutustunut [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) -palvelussa johdanto laitehallintaan, joka opastaa sinua laitteiden saamiseen Azure AD:n hallintaan.
2. Jos rekisteröit laitteita suoraan Azure AD:lle ja rekisteröit ne Intuneen, sinun on varmistettava, että olet määrittänyt [Intunen](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ja että käyttöoikeudet ovat ensin käytössä. [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support)
3. Varmista, että sinulla on oikeus suorittaa Azure AD:n ja paikallisen AD:n toimintoja. Vain Azure AD:n yleinen järjestelmänvalvoja voi hallita laiterekisteröinnin asetuksia. Lisäksi jos määrität automaattisia rekisteröintejä paikalliseen Active Directoryyn, sinun on oltava Active Directoryn ja AD FS:n järjestelmänvalvoja (jos sovellettavissa).

Azure AD -yhdistelmäliitoksen rekisteröintiprosessi edellyttää, että laitteet ovat yritysverkossa. Se toimii myös VPN-yhteyden kautta, mutta siihen on joitakin varoita. Olemme kuulleet, että asiakkaat tarvitsevat apua Azure AD-yhdistelmäympäristön rekisteröintiprosessin vianmäärityksessä etätyösyissä.

**Pilvitodennusympäristö (Azure AD:n salasanojen hash-synkronoinnin tai läpikäymisen todentamisen avulla)**

Tätä rekisteröintivirtaa kutsutaan myös nimellä "Synkronoi liity".

Seuraavassa on erittely rekisteröintiprosessin aikana tapahtuu:

1. Windows 10 service connection point (SCP) -tietueen, kun käyttäjä kirjautuu laitteeseen.

    1. Laite yrittää ensin noutaa asiakaspuolen SCP-tiedot rekisteristä [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Lisätietoja on [asiakirjassa.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    1. Jos se epäonnistuu, laite kommunikoi paikallisen Active Directoryn kanssa ja saa vuokraajan tiedot SCP:stä. Voit tarkistaa SCP:n viittaamalla tähän [asiakirjaan.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    > [!NOTE]
    > On suositeltavaa ottaa SCP käyttöön Active Directoryssa ja käyttää vain asiakaspuolen SCP-protokollaa alkuperäisen kelpoisuuden tarkistamisen aikana.

2. Windows 10 yrittää viestiä Azure AD:n kanssa järjestelmän kontekstissa ja todentaa itsensä Azure AD:n avulla.

    Voit tarkistaa, voiko laite käyttää Järjestelmätilin Microsoft-resursseja Test [Device Registration Connectivity -komentosarjan avulla.](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)

3. Windows 10 luo itse allekirjoitetun varmenteen ja tallentaa sen paikallisen Active Directoryn tietokoneobjektiin. Tämä edellyttää toimialueen ohjauskoneeseen näköyhteyttä.

4. Varmennetta saanut laiteobjekti synkronoidaan Azure AD:een Azure AD:n Näyttöyhteys. Synkronointijakso on oletusarvoisesti 30 minuutin välein, mutta se riippuu Azure AD Näyttöyhteys. Lisätietoja on tässä [asiakirjassa.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. Tässä vaiheessa aihelaitteen pitäisi nyt olla Odottaa-tilassa Azure Portalin Laite-kohdassa.

6. Kun seuraava käyttäjä kirjautuu Windows 10, rekisteröinti on valmis.

    > [!NOTE]
    > Jos käytät VPN-yhteyttä ja kirjautuminen ulos tai kirjautuminen lopettaa toimialueen yhteyden, voit käynnistää rekisteröinnin manuaalisesti. Voit tehdä tämän näin:
    >
    > Voit antaa `dsregcmd /join` paikallisen järjestelmänvalvojan kehotteen tai etäyhteyden PSExec-kehotteen kautta tietokoneeseesi.
    >
    > Esimerkki: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Yleisiä ongelmia laitteiden Azure Active Directory rekisteröinnissä on kohdassa Laitteiden usein [kysytyt kysymykset.](https://docs.microsoft.com/azure/active-directory/devices/faq)
