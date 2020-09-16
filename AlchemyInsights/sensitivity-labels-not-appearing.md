---
title: Herkkyys Tunnisteet eivät ilmesity
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801181"
---
# <a name="sensitivity-labels-not-appearing"></a>Herkkyys Tunnisteet eivät ilmesity

Herkkyys merkintöjen avulla voit luokitella ja suojata arkaluontoista sisältöä. Ne voidaan luoda Microsoft 365-yhteensopivuus keskuksessa, Microsoft 365-tieto turva keskuksessa tai Microsoft 365-tieto turva & yhteensopivuus keskuksessa luokittelu > herkkyys-selitteissä. Lisä tietoja tästä ominaisuudesta on artikkelissa [herkkyys merkkien yleiskatsaus](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Jos olet määrittänyt luottamuksellisuustunnisteet, mutta ne eivät näy Microsoft 365-sovelluksissa, tarkista seuraavat asiat:

- Varmista, että luottamuksellisuustarra on [julkaistu](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) käyttäjille ja ryhmille, jotka haluat määrittää.

- Varmista, että käyttäjä käyttää sovellusta, joka tukee herkkyys otsikoita-Katso [asia kirjan herkkyys otsikoita](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Jos olet [siirtämässä Azure-tieto turva-otsikoita](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), ota huomioon [tässä](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)luetellut seikat.

- Tietojen menetyksen estämisen (DLP) tuki: tällä hetkellä DLP-käytäntöjen ehtona voidaan käyttää vain säilytys otsikoita.  DLP-käytäntöjen luottamuksellisuusmerkintöjen tuki ei ole vielä käytettävissä, mutta työskentelemme sen parissa.

- Kun salaus on otettu käyttöön luottamuksellisuustarrassa, voit valita jommankumman seuraavista:
    - Määritä käyttö oikeudet nyt
    - Salli käyttäjien määrittää käyttö oikeuksia


Lisä tietoja mahdollisista ongelmista on kohdassa [arkaluonteisiin tunniste tietoihin liittyvät tunnetut ongelmat](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).