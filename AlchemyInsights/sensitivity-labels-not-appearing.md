---
title: Herkkyys merkinnät eivät näy
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 67719380aea0481f96c03fa591542e8e5a6e6993
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048649"
---
# <a name="sensitivity-labels-not-appearing"></a>Herkkyys merkinnät eivät näy

Herkkyys tunnisteiden avulla voit luokitella arkaluontoista sisältöä ja suojata sen. Ne voidaan luoda Microsoft 365 Compliance Centerissä, Microsoft 365 tieto turva keskuksessa tai Office 365 Security & Compliance Centerissa luokittelu > herkkyys merkintöjen alla. Lisä tietoja tästä ominaisuudesta on kohdassa [herkkyys merkintöjen yleiskuvaus](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).

Jos olet määrittänyt herkkyys Tunnisteet, mutta ne eivät näy Office-sovelluksissa, tarkista seuraavat seikat:

- Varmista, että herkkyys tarra on [julkaistu](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) haluamilleen käyttäjille ja ryhmille.

- Varmista, että käyttäjä käyttää sovellusta, joka tukee herkkyys tarroja – Katso [asia kirjan herkkyys tarrat](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).

- Jos olet [siirtamassa Azure Information Protection-tunnisteita](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), Huomaa [tässä](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)luetellut seikat.

- Tietojen menetyksen estämisen (DLP) tuki: tällä hetkellä vain säilytys tarroja voidaan käyttää ehtona DLP-käytännöissä.  DLP-käytännön herkkyys merkintöjen tuki ei ole vielä saatavilla, mutta työskentelemme sen parissa.

- Kun salaus on otettu käyttöön herkkyys merkinnässä, voit valita joko:
    - Määritä käyttö oikeudet nyt
    - Anna käyttäjien määrittää käyttö oikeuksia


Lisä tietoja mahdollisista ongelmista [on aiheessa herkkyys otsikoihin liittyvät tunnetut ongelmat](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).