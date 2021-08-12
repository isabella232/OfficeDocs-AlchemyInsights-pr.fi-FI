---
title: Luottamuksellisuusmerkinnät eivät näy
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
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061429"
---
# <a name="sensitivity-labels-not-appearing"></a>Luottamuksellisuusmerkinnät eivät näy

Luottamuksellisuusotsikoiden avulla voit luokitella ja suojata luottamuksellista sisältöäsi. Ne voidaan luoda tietoturvakeskuksen Microsoft 365 -yhteensopivuuskeskus Microsoft 365 tietoturvakeskuksessa tai Microsoft 365 yhteensopivuuskeskuksen & kohdassa Luokitus- > luottamuksellisuusmerkinnät. Lisätietoja tästä ominaisuudesta on kohdassa [Luottamuksellisuusotsikoiden yleiskatsaus.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)

Jos olet määrittänyt luottamuksellisuusmerkinnät, mutta ne eivät näy Microsoft 365 sovelluksissa, tarkista seuraavat asiat:

- Varmista, että luottamuksellisuusmerkintä [on julkaistu](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) haluamallasi käyttäjillä ja ryhmillä.

- Varmista, että käyttäjä käyttää sovellusta, joka tukee luottamuksellisuus otsikoita – katso [luottamuksellisuusmerkinnät asiakirjassa.](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)

- Jos olet [muuttamassa Azure Information Protection -tunnisteita](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), ota huomioon tässä luetellut [seikat.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- Tietojen menetyksen estäminen (DLP) -tuki: Tällä hetkellä vain säilytysotsikoita voidaan käyttää ehtona DLP-käytännöistä.  DLP-käytännön luottamuksellisuusotsikoiden tuki ei ole vielä käytettävissä, mutta työskentelemme sen kanssa.

- Kun salaus on otettu käyttöön luottamuksellisuusmerkinnässä, voit valita seuraavista:
    - Käyttöoikeuksien määrittäminen nyt
    - Käyttöoikeuksien määrittämisen salliminen käyttäjille


Lisätietoja mahdollisista ongelmista on kohdassa [Luottamuksellisuusotsikoiden tunnetut ongelmat](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).