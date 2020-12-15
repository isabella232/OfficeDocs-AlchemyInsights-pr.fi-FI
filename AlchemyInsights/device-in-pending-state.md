---
title: Laite odottaa-tilassa
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
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/11/2020
ms.locfileid: "49678480"
---
# <a name="device-in-pending-state"></a>Laite odottaa-tilassa

**Edellytykset**

1. Jos olet määrittämässä laitteiden rekisteröintejä ensimmäistä kertaa, varmista, että olet tarkistanut [laitteen hallinnan käytön Azure Active Directoryssa (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , joka ohjaa sinua käyttämään laitteita Azure AD:n hallinnassa.
2. Jos olet rekisteröimässä laitteita Azure AD:hen suoraan ja rekisteröimällä ne Intuneen, sinun on varmistettava, että olet [määrittänyt Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ja että [käyttö oikeus](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) on ensin käytössä.
3. Varmista, että sinulla on oikeus suorittaa toimintoja Azure AD:ssä ja paikallisessa MAINOKSESSA. Vain Azure AD:ssä oleva yleinen hallinnoija voi hallita laite rekisteröintien asetuksia. Lisäksi jos määrität automaattisia rekisteröintejä paikallisessa Active Directoryssa, sinun on oltava Active Directoryn ja AD FS:N järjestelmänvalvoja (tarvittaessa).

Hybridi Azure AD Join-rekisteröinti prosessi edellyttää, että laitteet ovat yrityksen verkossa. Se toimii myös VPN-yhteyden kautta, mutta siihen liittyy joitakin varoituksista. Olemme kuulleet, että asiakkaat tarvitsevat apua vian määrityksessä hybridi Azure AD Join-rekisteröinti prosessissa etätyöolosuhteissa.

**Pilvi todennus ympäristö (Azure AD Password hash-synkronoinnin tai läpi vienti todennuksen avulla)**

Tätä rekisteröinti kulkua kutsutaan myös nimellä "synkronointi liitos".

Tässä on erittely siitä, mitä rekisteröinti prosessin aikana tapahtuu:

1. Windows 10 havaitsee palvelun yhteys pisteen (SCP) tietueen, kun käyttäjä kirjautuu laitteeseen.

    1. Laite yrittää ensin hakea vuokra ajan tietoja asiakas puolen SCP-rekisteristä [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Lisä tietoja on kohdassa [asia kirja](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Jos se epäonnistuu, laite kommunikoi paikallisen Active Directoryn kanssa ja saa vuokra ajan tietoja SCP-tieto kannasta. Jos haluat tarkistaa SCP-tiedoston, Lue tämä [asia kirja](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Suosittelemme, että SCP otetaan käyttöön Active Directoryssa ja että se on käytössä vain asiakas puolen SCP: ssa alkuperäistä vahvistusta varten.

2. Windows 10 yrittää muodostaa yhteyden Azure AD:hen järjestelmä kontekstissa ja todentaa itsensä Azure AD:hen.

    Voit tarkistaa, Voiko laite käyttää Microsoft-resursseja järjestelmä tilillä, käyttämällä [testi laitteen rekisteröinnin yhteys komento sarjaa](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 luo itse allekirjoitetun varmenteen ja tallentaa sen paikallisen Active Directoryn tieto kone-objektiin. Tämä edellyttää näkö yhteys toimi alueen ohjaus koneeseen.

4. Laite objekti, jonka varmenne on synkronoitu Azure AD:hen Azure AD Connectin kautta. Synkronointi sykli on oletusarvoisesti 30 minuutin välein, mutta se määräytyy Azure AD Connectin määritysten mukaan. Jos haluat lisä tietoja, Lue tämä [asia kirja](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Tässä vaiheessa sinun pitäisi pystyä näkemään aihe laite "**odottaa**"-tilassa, joka on Azure-portaalin Device Blade-kohdassa.

6. Kun seuraava käyttäjä on kirjautunut Windows 10: een, rekisteröinti valmistuu.

    > [!NOTE]
    > Jos käytät VPN-yhteyttä ja uloskirjautuminen/Kirjautuminen lopettaa toimi alueen yhdistämisen, voit laukaista rekisteröinnin manuaalisesti. Voit tehdä sen seuraavasti:
    >
    > Ongelma `dsregcmd /join` paikallisesti järjestelmänvalvojan kehotteessa tai etäyhteyden kautta PSExec tieto koneeseen.
    >
    > Esimerkki: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Yleisiä ongelmia Azure Active Directory-laitteen rekisteröinnissä on kohdassa [laitteiden usein kysytyt kysymykset](https://docs.microsoft.com/azure/active-directory/devices/faq).
