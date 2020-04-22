---
title: Officen käyttöönottotyökalun käyttäminen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726245"
---
# <a name="using-the-office-deployment-tool-odt"></a>Officen käyttöönottotyökalun (ODT) käyttäminen

Office 365 -version käyttöönotto on office-käyttöönottotyökalua (ODT) käyttämällä. Officen käyttöönottotyökalu (setup.exe) suoritetaan komentoriviltä, ja sen avulla määritetään xml-määritystiedoston avulla, mitä asetuksia Officen käyttöönotossa käytetään.
  
1. Lataa Officedeployment Tool -työkalun uusin versio [Microsoft Download Centeristä](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Valitse käyttöönottoasetukset ja luo xml-määritystiedosto [Officecustomization Tool (OCT) -työkalun](https://config.office.com) avulla. Vie määritystiedosto ja sijoita se paikallisesti samaan kansioon, jossa setup.exe sijaitsee.

    **Huomautus:** Officen asennusongelmia ilmenee yleensä virheellisesti määritettyjen tai väärin muotoiltujen määritystiedostojen vuoksi. Tällaisten ongelmien välttämiseksi on suositeltavaa luoda määritystiedosto Officen mukautustyökalun avulla. Voit myös tuoda aiemmin luotuja määritystiedostoja Officen mukautustyökaluun.

3. Siirry laajennetusta komentorivistä sijaintiin, jossa setup.exe sijaitsee, ja suorita Officedeployment Tool lataustilassa ja määritä juuri tallentamasi määritystiedosto. Tässä esimerkissä määritystiedoston nimi on Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Suorita Officen käyttöönottotyökalu määritystilassa ja määritä määritystiedosto.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Huomautus:** Sinun on suoritettava tämä vaihe asiakastietokoneesta, johon haluat asentaa Officen, ja sinulla on oltava paikallisen järjestelmänvalvojan oikeudet kyseiseen tietokoneeseen.

Lisätietoja Officedeployment Tool -työkalun käyttämisestä Microsoft 365 Apps for enterprise -käyttöönottoskenaarioissa on artikkelissa [Officen käyttöönottotyökalun yleiskatsaus](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Lisätietoja Officen mukautustyökalun käyttämisestä on artikkelissa [Officen mukautustyökalun yleiskatsaus](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
