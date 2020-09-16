---
title: Asiakkaan todennus varmenteen käyttöönoton vian määritys
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
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658983"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Asiakkaan todennus varmenteen käyttöönoton vian määritys

Intune NDES/SCEP-ja PKCS/PFX-asiakas sertifikaattien profiileja käytetään yleisesti yhdessä muiden profiilien kanssa, kuten WiFi, VPN ja Sähkö posti, jotta käyttäjät voivat todentaa yrityksen resurssit. Kun nämä profiili tyypit on linkitetty asiakas sertifikaatti profiiliin, ne määräytyvät kyseisen profiilin onnistuneen käyttöönoton mukaan.

Alkuperäisen infrastruktuurin määrittäminen ja siihen liittyvät asiakas sertifikaatti profiilin määritykset vaativat usein vian määritystä. Vaiheittaiset ohjeet NDES-yhdistimen onnistuneeseen määrittämiseen ja vian määritys ohjeisiin varmenteen käyttöönottoon liittyvien ongelmien eristämiseksi on kohdassa: 

- [Infrastruktuurin määrittäminen tuke, jos haluat, että SCEP on Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Yleistä SP-varmenne profiilien vian määrityksestä Microsoft Intunella](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Käytä viitattua PowerShell-komento sarjoja määritysten vahvistamiseen. Lisä tietoja on kohdassa [Intune-varmenne liittimen tarkistus komento sarjat](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Muita yleisiä ongelmia**

**Kun yritän asentaa Intune-varmenne yhdistimen NDES Connector Server-palvelimeen, näyttöön tulee sanoma "varmenne pyynnön Sala sanaa ei voi vahvistaa. Sitä on ehkä jo käytetty. Hanki uusi sala sana, jotta voit lähettää pyynnön tällä pyynnöllä. "**  

Tämä viesti tarkoittaa, että sinun on suoritettava varmenne liittimen asennus järjestelmänvalvojana.

Joissain ympäristöissä palvelinten, joissa Intune-varmenne suoritetaan, tulee käyttää välitys palvelinta yhteyden muodostamiseen Intuneen, joten varmenne yhdistimen on käytettävä välitys palvelinta. Joissakin tapa uksissa NDES-yhdistin ohittaa määritetyt välitys palvelimen asetukset ja saattaa olla tarpeen määrittää välitys palvelimen asetukset, kun ne suoritetaan LocalSystem-tieto turva kontekstissa. 
 
Ratkaisu on käyttää Internet Exploreria JÄRJESTELMÄNÄ ja määrittää välitys palvelimen IE:Ä. Kun Intune Connector-palvelu käynnistetään uudelleen, NDES-yhdistin muodostaa yhteyden Intuneen.

**Käyttäjä laitteet eivät enää saa SCEP-varmenteita NDESIN kautta.**

On mahdollista, että NDES-palvelimelle myönnetty asiakkaan todennus varmenne, joka on määritetty NDES Connector-asennuksen aikana, on vanhentunut tai puuttuu. Voit korjata ongelman seuraavasti: 
 
1. Poista NDES-yhdistimen asennus.  
2. Näiden tietojen avulla voit pyytää uutta asiakas todentamista tai palvelimen todennus varmennetta: 
 
    - Aiheen nimi: CN = External täydellinen  
    - Aihe Vaihtoehtoinen nimi (molemmat ovat pakollisia): DNS = External täydellinen, DNS = Internal täydellinen 
 
3. Asenna NDES-yhdistin uudelleen uuteen sertifikaattiin.