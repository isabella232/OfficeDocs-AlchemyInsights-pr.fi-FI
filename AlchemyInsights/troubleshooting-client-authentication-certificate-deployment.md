---
title: Asiakastodennusvarmenteen käyttöönoton vianmääritys
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020801"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Asiakastodennusvarmenteen käyttöönoton vianmääritys

Intune NDES/SCEP- ja PKCS/PFX Client -varmenteiden profiileja käytetään yleisesti muiden profiilityyppien, kuten WiFi-, VPN- ja sähköpostiprofiilien, kanssa, jotta käyttäjät voivat todentaa tiedot yrityksen resursseihin. Kun nämä profiilityypit on linkitetty asiakasvarmenneprofiiliin, riippuu profiilin onnistuneesta käyttöönotosta.

Alkuinfrastruktuurimääritys ja siihen liittyvä asiakasvarmenneprofiilin määritys edellyttävät usein vianmääritystä. Vaiheittaiset ohjeet NDES-yhdistimen onnistuneeseen määritykseen ja vianmääritysohjeet varmenteen käyttöönottoongelmien eristämiseen ovat seuraavassa: 

- [Infrastruktuurin määrittäminen SCEP:n tueksi Intunen avulla](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Yleistä SCEP-varmenneprofiilien vianmäärityksestä Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Käytä viitattuja PowerShell-komentosarjoja kokoonpanon vahvistamiseen. Lisätietoja on kohdassa [Intune-varmenteen yhdistimen vahvistuskomentosarjat.](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)

  
**Muita yleisiä ongelmia**

**Kun yritän asentaa Intune-varmenteen yhdistimen NDES-yhdistinpalvelimeen, näyttöön tulee sanoma "Varmennepyynnön salasanaa ei voida vahvistaa. Sitä on ehkä jo käytetty. Hanki uusi salasana tämän pyynnön lähettämistä varten."**  

Tämä sanoma tarkoittaa, että varmenneyhdistimen asennus on suoritettava järjestelmänvalvojana.

Joissakin ympäristöissä palvelimissa, joissa Intune-varmenne suoritetaan, on muodostettava yhteys Intuneen välityspalvelimen avulla, joten varmenteen yhdistimen on käytettävä välityspalvelinta. Joissakin tilanteissa NDES-yhdistin ohittaa määritetyt välityspalvelimen asetukset, ja välityspalvelimen asetukset on ehkä määritettävä, kun ne suoritetaan LocalSystemin suojauskontekstissa. 
 
Ratkaisuna on suorittaa Internet Explorer SYSTEM -palvelimeksi ja määrittää välityspalvelin IE:ssä. Intune-yhdistinpalvelun uudelleenkäynnistyksen jälkeen NDES-yhdistin muodostaa yhteyden Intuneen.

**Käyttäjälaitteet eivät enää saa SCEP-varmenteita NDES-palvelusta.**

On mahdollista, että NDES-palvelimelle myönnetty asiakkaan todennusvarmenne, joka on määritetty NDES-yhdistimen asennuksen aikana, on vanhentunut tai puuttuu. Ratkaiseminen: 
 
1. Poista NDES-yhdistimen asennus.  
2. Näiden tietojen avulla voit pyytää uutta asiakkaan todennusta tai palvelimen todennusvarmennetta: 
 
    - Aiheen nimi: CN=external fqdn  
    - Aiheen vaihtoehtoinen nimi (molemmat ovat pakollisia): DNS=external fqdn, DNS=internal fqdn 
 
3. Asenna NDES-yhdistin uudelleen uudella varmenteella.