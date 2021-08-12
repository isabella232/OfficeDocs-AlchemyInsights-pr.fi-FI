---
title: PRT-ongelman vianmääritys
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: fd285d1158d7b358e4c698cf6014422cc2fb536e1fbdf98630bebda359f9c553
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972713"
---
# <a name="troubleshoot-prt-issue"></a>PRT-ongelman vianmääritys

Jotta mikä tahansa laite voidaan todentaa, sen on oltava täysin rekisteröity ja hyvässä kunnossa ja se on hankittava ensisijainen päivitystunnus (PRT).

Azure AD -yhdistelmäliitoksen rekisteröintiprosessi edellyttää, että laitteet ovat yritysverkossa. Se toimii myös VPN-yhteyden kautta, mutta siihen on joitakin varoita. Olemme kuulleet, että asiakkaat tarvitsevat apua Azure AD-yhdistelmäympäristön rekisteröintiprosessin vianmäärityksessä etätyösyissä. Tässä on erittely siitä, mitä rekisteröintiprosessin aikana tapahtuu "hupun alla".

**Pilvitodennusympäristö (Azure AD:n salasanojen hash-synkronoinnin tai läpikäymisen todentamisen avulla)**

Tätä rekisteröintivirtaa kutsutaan myös nimellä "Synkronoi liity".

1. Windows 10 löytää SCP-tietueen, kun käyttäjä kirjautuu laitteeseen.
    1. Laite yrittää ensin noutaa asiakaspuolen SCP-tiedot rekisteristä [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Lisätietoja on tässä [asiakirjassa.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    2. Jos se epäonnistuu, laite kommunikoi paikallisen Active Directoryn (AD) kanssa ja saa vuokraajan tiedot SCP (Service Connection Point) -palvelusta. Jos haluat tarkistaa SCP:n, katso tätä [asiakirjaa.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

> [!NOTE]
> On suositeltavaa ottaa SCP käyttöön AD:ssä ja käyttää vain asiakaspuolen SCP-protokollaa alkutarkistusta varten.

2. Windows 10 yrittää viestiä Azure AD:n kanssa järjestelmän kontekstissa ja todentaa itsensä Azure AD:n avulla. Voit tarkistaa, voiko laite käyttää järjestelmätilin Microsoft-resursseja Test Device Registration Connectivity -komentosarjan avulla.

3. Windows 10 luo itse allekirjoitetun varmenteen ja tallentaa sen paikallisen AD:n tietokoneobjektiin. Tämä edellyttää toimialueen ohjauskoneeseen näköyhteyttä.

4. Laiteobjekti, jolla on varmenne, synkronoidaan Azure AD:lle Azure AD:n Näyttöyhteys. Synkronointijakso on oletusarvoisesti 30 minuutin välein, mutta se riippuu Azure AD :n Näyttöyhteys. Lisätietoja on tässä [asiakirjassa.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. Tässä vaiheessa aihelaitteen pitäisi nyt olla Odottaa-tilassa Azure Portalin Laite-kohdassa.

6. Kun seuraava käyttäjä kirjautuu Windows 10, rekisteröinti on valmis. 

> [!NOTE]
> Jos käytät VPN-yhteyttä ja kirjautumisprosessi lopettaa toimialueyhteyden, voit käynnistää rekisteröinnin manuaalisesti:
 1. Voit antaa dsregcmd /join paikallisesti järjestelmänvalvojan kehotteeseen tai etäyhteyden kautta PSExec-yhteydellä tietokoneeseen. Esimerkiksi PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Lisätietoja yhdistelmäliitoksen ongelmista on kohdassa Laitteiden [ongelman vianmääritys.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
