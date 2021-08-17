---
title: Käyttöönottotyökalun Office käyttäminen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083767"
---
# <a name="using-the-office-deployment-tool-odt"></a>Office käyttöönottotyökalun (ODT) käyttäminen

Voit ottaa Office (ODT) -työkalulla käyttöön Office 365 versioista Office. Office käyttöönottotyökalu (setup.exe) suoritetaan komentoriviltä ja sen avulla määritetään XML-määritystiedostoa ottamalla käyttöön Office.
  
1. Lataa Office-käyttöönottotyökalun uusin versio Microsoft [Download Centeristä.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. Valitse [käyttöönottoasetukset Office mukauttamistyökalun (OCT)](https://config.office.com) avulla ja luo xml-määritystiedosto. Vie määritystiedosto ja sijoita se paikallisesti samaan kansioon, jossa setup.exe sijaitsee.

    **Huomautus:** Office asennusongelmia ilmenee yleisesti virheellisesti määritettyjen tai väärin muotoiltujen määritystiedostojen vuoksi. Tällaisten ongelmien välttämiseksi suosittelemme, että luot määritystiedoston Office mukautustyökalulla. Voit myös tuoda aiemmin luotuja määritystiedostoja Office mukauttamistyökaluun.

3. Siirry järjestelmänvalvojan oikeuksin suoritettavasta komentokehotteesta sijaintiin, jossa setup.exe sijaitsee, suorita Office-käyttöönottotyökalu lataustilassa ja määritä juuri tallennettu määritystiedosto. Tässä esimerkissä määritystiedoston nimi on Configuration.xml:

```setup.exe /download Configuration.xml```

4.Suorita Office-käyttöönottotyökalu määritystilassa ja määritä määritystiedosto.

```setup.exe /configure Configuration.xml```

**Huomautus:** Tämä vaihe on suoritettava sen asiakastietokoneen kautta, johon haluat asentaa Office ja sinulla on oltava paikallisen järjestelmänvalvojan oikeudet tähän tietokoneeseen.

Lisätietoja Office käyttöönottotyökalun käyttämisestä Microsoft 365 -sovellukset suuryrityksille käyttöönottoskenaarioissa on ohjeaiheessa Yleistä [Office käyttöönottotyökalusta.](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) Lisätietoja mukautustyökalun Office on kohdassa Office [yleiskatsaus.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)
