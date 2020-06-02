---
title: 1491-haku-ei-palaa-odotettu-tulokset
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
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510569"
---
# <a name="content-search-not-returning-expected-results"></a>Sisältöhaku ei palauta odotettuja tuloksia

Kun suoritat sisältöhakuja Microsoft 365:n tietoturva- & Compliance Centeristä, saatat saada odottamattomia hakutuloksia. Mieti seuraavia asioita, jotka voivat vaikuttaa hakutuloksiin:

- **Sisältösijainnit ja hakuehdot**: Varmista, että olet valinnut oikeat sisältösijainnit ja hakuehdot. Jos teit suuren haun (jossa on useita sijainteja), harkitse sen jakamista useisiin hakuihin.

- **Osittain indeksoidut kohteet:** Postilaatikoiden [osittain indeksoidut kohteet](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) sisältyvät arvioituihin hakutuloksiin. SharePointin ja OneDriven sivustojen osittain indeksoidut kohteet eivät kuitenkaan sisälly hakuarvioon.

- **Hakuvirheet**: Kun etsit suurta määrää postilaatikoita (yli 100 000 postilaatikkoa), saatat saada hakuvirheitä virhekoodeilla, kuten CS008-009 ja CS012-002). Yritä tässä tapauksessa etsiä vain epäonnistuneita sisältösijainteja uudelleen. Lisätietoja [on tässä artikkelissa.](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search)
