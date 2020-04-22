---
title: 1491-haku-ei-palaa odotettu-tulokset
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709224"
---
# <a name="content-search-not-returning-expected-results"></a>Sisältöhaku ei palauta odotettuja tuloksia

Kun suoritat sisältöhakuja Microsoft 365:n tietoturva- & yhteensopivuuskeskuksesta, näyttöön saattaa tulla odottamattomia hakutuloksia. Mieti seuraavia seikkoja, jotka voivat vaikuttaa hakutuloksiin:

- **Sisällön sijainnit ja hakuehdot**: Varmista, että olet valinnut oikeat sisältösijainnit ja hakuehdot. Jos olet etsinyt suurta hakua (jossa on useita sijainteja), harkitse sen jakamista useisiin hakuihin.

- **Osittain indeksoituja kohteita:** [Osittain indeksoituja postilaatikoiden kohteita](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) sisällytetään arvioituihin hakutuloksiin. Osittain indeksoituja kohteita SharePointin ja OneDriven sivustoista ei kuitenkaan sisällytetä hakuarvioon.

- **Hakuvirheet**: Etsiessäsi suurta määrää postilaatikoita (yli 100 000 postilaatikkoa) saatat saada hakuvirheitä, joissa on virhekoodeja, kuten CS008-009 ja CS012-002). Yritä tässä tapauksessa etsiä vain epäonnistuneiden sisältösijaintien hakua. Lisätietoja on [tässä artikkelissa.](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search)
