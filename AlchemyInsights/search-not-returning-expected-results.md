---
title: 1491-search-not-returning-expected-results
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
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052707"
---
# <a name="content-search-not-returning-expected-results"></a>Sisältöhaku ei palauta odotettuja tuloksia

Kun sisältöhakuja suoritetaan Microsoft 365 tietoturva- & yhteensopivuuskeskuksesta, saatat saada odottamattomia hakutuloksia. Ota huomioon seuraavat asiat, jotka voivat vaikuttaa hakutuloksiin:

- **Sisällön sijainnit ja hakuehdot:** Varmista, että olet valinnut oikeat sisältösijainnit ja hakuehdot. Jos olet etsinyt paljon (ja sinulla on useita sijainteja), voit jakaa sen useisiin hakuihin.

- **Osittain indeksoidut kohteet:**  [Postilaatikoiden](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) osittain indeksoidut kohteet sisällytetään arvioituihin hakutuloksiin. Indeksoidut kohteet eivät kuitenkaan sisälly hakuarvioon SharePoint OneDrive indeksoiduista sivustoista.

- **Hakuvirheet:** Kun haet suurta määrää postilaatikoita (yli 100 000 postilaatikkoa), hakuvirheitä voi i olla, ja virhekoodit, kuten CS008-009 ja CS012-002). Tässä tapauksessa yritä hakea uudelleen vain epäonnistuneita sisältösijainteja. Lisätietoja  [on tässä](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) artikkelissa.
