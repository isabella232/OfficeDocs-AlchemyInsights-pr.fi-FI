---
title: Asiakkaan todennusvarmenteen käyttöönoton vianmääritys
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555001"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Asiakkaan todennusvarmenteen käyttöönoton vianmääritys

Intune NDES/SCEP- ja PKCS/PFX-asiakassertifikaattiprofiileja käytetään yleisesti yhdessä muiden profiilityyppien, kuten Wifin, VPN:n ja sähköpostin, kanssa, jotta käyttäjät voivat todentaa yrityksen resurssit. Kun nämä profiilityypit on linkitetty asiakassertifikaattiprofiiliin, se riippuu kyseisen profiilin onnistuneesta käyttöönotosta.

Asiakassertifikaattiprofiilin alkuinfrastruktuurin asetukset ja siihen liittyvät määritykset edellyttävät usein vianmääritystä. Vaiheittaiset ohjeet NDES-liittimen onnistuneeseen asennukseen ja vianmääritysohjeet varmenteiden käyttöönottoon liittyvien ongelmien eristämiseksi ovat seuraavissa ohjeissa: 

- [Määritä infrastruktuuri tukemaan SCEP:tä Intunella](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Yleistä SCEP-varmenneprofiilien vianmäärityksestä Microsoft Intunen avulla](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Tarkista kokoonpano käyttämällä viitattuja powershell-komentosarjoja. Lisätietoja on kohdassa [Intune Certificate Connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Muita yleisiä kysymyksiä**

**Kun yritän asentaa Intune-varmenneliittimen NDES-yhdistinpalvelimeen, näyttöön tulee sanoma "Varmennepyynnön salasanaa ei voi vahvistaa. Sitä on ehkä jo käytetty. Hanki uusi salasana, jonka haluat lähettää tämän pyynnön yhteydessä."**  

Tämä sanoma tarkoittaa, että sertifikaattiyhdistimen asennus on suoritettava järjestelmänvalvojana.

Joissakin ympäristöissä palvelimissa, joissa Intune-varmenne suoritetaan, on käytettävä välityspalvelinta yhteyden muodostamiseen Intuneen, joten Varmenteen yhdistimen on käytettävä välityspalvelinta. Joissakin tapauksissa NDES Connector ohittaa määritetyt välityspalvelimen asetukset, ja välityspalvelimen asetukset on ehkä määritettävä paikallisen järjestelmän suojauskontekstissa. 
 
Liuos on jotta ajelu Jäsentenvälinen Tehdä tutkimusmatka koska ELIMISTÖ ja configure valtuutettu edustaja kotona IE. Kun Intune Connector Service on käynnistetty uudelleen, NDES-liitin muodostaa yhteyden Intuneen.

**Käyttäjälaitteet eivät enää saa SCEP-sertifikaatteja NDES:ltä.**

On mahdollista, että NDES-palvelimelle myönnetty ja NDES-yhdistimen asennuksen aikana määritetty asiakkaan todennusvarmenne on vanhentunut tai puuttuu. Voit ratkaista ongelman: 
 
1. Poista NDES-liittimen asennus.  
2. Näiden tietojen avulla voit pyytää uutta asiakkaan todennus- tai palvelimen todennusvarmennetta: 
 
    - Aiheen nimi: CN=external fqdn  
    - Aihe vaihtoehtoinen nimi (molemmat ovat pakollisia): DNS=ulkoinen fqdn, DNS=sisäinen fqdn 
 
3. Asenna NDES-liitin uudelleen uudella varmenteella.