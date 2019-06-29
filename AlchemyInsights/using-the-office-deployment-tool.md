---
title: Office Deployment-työkalun avulla
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 998f914f38fa9d1925f7003e634d7f11550f47da
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365522"
---
# <a name="using-the-office-deployment-tool-odt"></a>Office Deployment Tool (ODT-työkalun) avulla

Office Deployment Tool (ODT) avulla voit ottaa käyttöön Office-version Office 365: ssä. Office Deployment Tool-työkalua (setup.exe) suoritetaan komentoriviltä, ja selvittää, mitä asetuksia, voit ottaa käyttöön Office XML-määritystiedoston avulla.
  
1. Lataa uusin versio Office Deployment Tool-työkalua [Microsoft Download Centeristä](http://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Luo XML-määritystiedosto ja valitse käyttöönoton asetukset [Office Customization Tool (OCT)](https://config.office.com) avulla. Määritystiedoston vieminen ja sijoittaa sen paikallisesti samaan kansioon, jossa asuu setup.exe.

    **Huomautus:** Office-asennuksen ongelmista esiintyy yleisesti asianmukaisesti, sen kokoonpano on väärä tai malformatted määritystiedostoja. Tällaisten ongelmien välttämiseksi on suositeltavaa, että käytät Officen mukauttamistyökalun määritystiedoston luominen. Voit myös tuoda aiemmin luotuja määritystiedostoja Officen mukauttamistyökalun.

3. Siirry sijaintiin, jossa asuu setup.exe järjestelmänvalvojan oikeuksin suoritettava komentorivi ja suorita Office Deployment Tool-työkalua download tilassa ja määrittää tiedoston juuri tallennettu. Tässä esimerkissä tiedoston nimi on Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Suorita Office Deployment Tool-työkalua ja määritä tila määrittää määritystiedoston.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Huomautus:** Tämä vaihe on suoritettava asiakastietokoneesta, johon haluat asentaa Officen ja sinulla on oltava paikallisen järjestelmänvalvojan oikeudet tietokoneeseen.

Saat lisätietoja Office Deployment Tool-työkalua käyttämällä Office 365 ProPlus käyttöönottoprosessissa on [Yleiskatsaus Office Deployment Tool-työkalua](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Lisätietoja Officen mukauttamistyökalun käyttämisestä on ohjeaiheessa [Officen mukauttamistyökalun yleiskatsaus](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
