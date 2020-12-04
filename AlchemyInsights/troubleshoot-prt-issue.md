---
title: PRT-ongelman vian määritys
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
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573495"
---
# <a name="troubleshoot-prt-issue"></a>PRT-ongelman vian määritys

Jotta kaikki laitteet saataisiin todennettua, niiden on oltava täysin rekisteröity ja hyvässä kunnossa ja niiden on pystyttävä hankkimaan ensisijaiset päivitys tunnus (PRT).

Hybridi Azure AD Join-rekisteröinti prosessi edellyttää, että laitteet ovat yrityksen verkossa. Se toimii myös VPN-yhteyden kautta, mutta siihen liittyy joitakin varoituksista. Olemme kuulleet, että asiakkaat tarvitsevat apua vian määrityksessä hybridi Azure AD Join-rekisteröinti prosessissa etätyöolosuhteissa. Seuraavassa on tietoja siitä, mitä kone pellin alle tapahtuu rekisteröinti prosessin aikana.

**Pilvi todennus ympäristö (Azure AD Password hash-synkronoinnin tai läpi vienti todennuksen avulla)**

Tätä rekisteröinti kulkua kutsutaan myös nimellä "synkronointi liitos".

1. Windows 10 havaitsee SCP-tietueen, kun käyttäjä kirjautuu laitteeseen.
    1. Laite yrittää ensin hakea vuokra ajan tietoja asiakas puolen SCP-rekisteristä [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Katso lisä tietoja tästä [asia kirjasta](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Jos se epäonnistuu, laite kommunikoi paikallisen Active Directoryn (AD) kanssa saadakseen vuokra ajan tietoja palvelun yhteys pisteestä (SCP). Jos haluat tarkistaa SCP-toiminnon, Lue tämä [asia kirja](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Suosittelemme, että SCP otetaan käyttöön MAINOKSESSA ja että se on käytössä vain asiakas puolen SCP: ssa alkuperäisen kelpoisuuden tarkistamista varten.

2. Windows 10 yrittää muodostaa yhteyden Azure AD:hen järjestelmä kontekstissa ja todentaa itsensä Azure AD:hen. Voit tarkistaa, Voiko laite käyttää Microsoft-resursseja järjestelmä tilillä, käyttämällä testi laitteen rekisteröinnin yhteys komento sarjaa.

3. Windows 10 luo itse allekirjoitetun varmenteen ja tallentaa sen paikallisessa MAINOKSESSA tieto kone-objektiin. Tämä edellyttää näkö yhteys toimi alueen ohjaus koneeseen.

4. Laite objekti, joka sisältää varmenteen, synkronoidaan Azure AD:hen Azure AD Connectin kautta. Synkronointi sykli on oletusarvoisesti 30 minuutin välein, mutta se määräytyy Azure AD Connectin määritysten mukaan. Katso lisä tietoja tästä [asia kirjasta](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Tässä vaiheessa sinun pitäisi pystyä näkemään aihe laite "odottaa"-tilassa, joka on Azure-portaalin Device Blade-kohdassa.

6. Kun seuraava käyttäjä on kirjautunut Windows 10: een, rekisteröinti valmistuu. 

> [!NOTE]
> Jos käytät VPN-yhteyttä ja kirjautuminen ulos-Kirjautumisprosessi lopettaa toimi alue yhteyden, voit käynnistää rekisteröinnin manuaalisesti:
 1. Ongelma dsregcmd/Join paikallisesti järjestelmänvalvojan kehotteesta tai etäyhteyden kautta PSExec tieto koneeseen. Esimerkiksi PsExec-n \\ win10client01 cmd, dsregcmd/Join

 2. Lisä tietoja yhdistelmä liitoksen ongelmista on kohdassa laitteet- [ongelman vian määritys](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
