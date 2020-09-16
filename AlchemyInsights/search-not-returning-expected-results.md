---
title: 1491-haku-ei-palautus-odotetut tulokset
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740471"
---
# <a name="content-search-not-returning-expected-results"></a>Sisältö haku ei palauta odotettuja tuloksia

Kun sisältö haut suoritetaan Microsoft 365-tieto turva & yhteensopivuus keskuksesta, näyttöön voi tulla odottamattomia haku tuloksia. Ota huomioon seuraavat asiat, jotka voivat vaikuttaa haku tuloksiin:

- **Sisältö sijainnit ja haku ehdot**: Varmista, että olet valinnut oikeat sisältö sijainnit ja haku ehdot. Jos suoritit suuren haun (monissa sijainneissa), harkitse sen jakamista useaan hakuun.

- **Osittain indeksoidut kohteet**:  [osittain indeksoidut kohteet](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) posti laatikoista sisällytetään arvio ituihin haku tuloksiin. Kuitenkin osittain indeksoidut kohteet SharePointin ja OneDriven kohteista eivät sisälly haku arvioon.

- **Haku**virheet: kun haet suurta määrää posti laatikoita (yli 100 000 posti laatikkoa), saatat saada haku virheitä, joissa on virhe koodit, kuten CS008-009 ja CS012-002). Tässä tapa uksessa yritä hakea vain epäonnistuneista sisältö sijainneista. Katso lisä tietoja  [tästä artikkelista](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .
