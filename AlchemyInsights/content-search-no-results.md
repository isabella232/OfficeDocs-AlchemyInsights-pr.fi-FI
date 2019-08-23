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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516776"
---
# <a name="no-results-from-content-searchexports"></a>Tuloksia-sisällön haku ja vienti

Ongelmia kanssa sisällön haku ja vienti tuota tietoja voi olla tiettyjen vaatimusten Suojaussuodatin, jonka oli asennuksen tiettyyn Admin ja ei toimi kaikki järjestelmänvalvojat.

Voit ratkaista ongelman, Tarkista ovatko noudattaminen suojaus-suodattimia, jotka saattavat aiheuttaa tämän:
1. Security and Compliance Centeriin PowerShellin muodostaa yhteyden
2. Suorita seuraavat commandlets:
<br>$org = ”yourdomain.com”
<br>Get-ComplianceSecurityFilter-$org-organisaatio