---
title: 1491-Search-not-returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: 881a579d7098578452c994b7ac66fe22a1d90dc2
ms.sourcegitcommit: 5182c9a73641079be59740e4524434b2e8be613a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29964851"
---
# <a name="content-search-not-returning-expected-results"></a>Tuota odotettuja tuloksia sisällöstä etsiminen

Kun sisällön hakujen suorittaminen Office 365: n suojauksen & Compliance Centeriin, näyttöön saattaa tulla odottamaton hakutuloksia. Ota huomioon seuraavat asiat, jotka vaikuttavat hakutulosten:

- **Sisällön sijainnit ja hakuehdot**: Varmista, että olet valinnut oikean sisällön sijainnit ja hakuehdot. Jos suoritit (useissa paikoissa) suuri etsintä, ota huomioon jakaminen useita hakuja.

- **Osittain Indeksoidut kohteet**: arvioidun hakutulosten postilaatikoista [osittain Indeksoidut kohteet](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) sisällytetään. Kuitenkin osittain indeksoidut objektit sivustojen SharePoint-ja OneDrive eivät sisälly Haku-arvio.

- **Etsi virheet**: Kun etsit on paljon (yli 100 000 postilaatikot) postilaatikoita, voit saada Etsi virheet, virhekoodit kuten CS008-009 ja CS012-002). Tässä tapauksessa yrittää vain epäonnistuneet sisällön sijaintien osalta. Katso lisätietoja [tämän artikkelin](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) .
