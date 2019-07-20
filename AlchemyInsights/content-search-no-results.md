---
title: Sisältö ei ole hakutulokset
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800314"
---
# <a name="no-results-from-content-searchexports"></a>Tuloksia-sisällön haku ja vienti

Ongelmia kanssa sisällön haku ja vienti tuota tietoja voi olla tiettyjen vaatimusten Suojaussuodatin, jonka oli asennuksen tiettyyn Admin ja ei toimi kaikki järjestelmänvalvojat.

Voit ratkaista ongelman, Tarkista ovatko noudattaminen suojaus-suodattimia, jotka saattavat aiheuttaa tämän:
1. Security and Compliance Centeriin PowerShellin muodostaa yhteyden
2. Suorita seuraavat commandlets:
<br>$org = ”yourdomain.com”
<br>Get-ComplianceSecurityFilter-$org-organisaatio