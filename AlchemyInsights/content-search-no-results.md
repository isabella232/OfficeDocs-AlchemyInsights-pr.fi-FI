---
title: Sisältöhaun tulokset eivät ole
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816845"
---
# <a name="no-results-from-content-searchexports"></a>Ei tuloksia sisältöhaun/vientien avulla

Sisältöhaun ja viennin ongelmat, jotka eivät palauta tietoja, voivat johtua tietyistä tietyn järjestelmänvalvojan määritysten yhteensopivuuden suojaussuodattimesta, joka ei ole ilmoittanut siitä kaikille järjestelmänvalvojille.

Voit ratkaista ongelman tarkistamaan, aiheuttavatko ne yhteensopivuuden suojaussuodattimet:
1. Yhteyden muodostaminen tietoturva- ja yhteensopivuuskeskuksen PowerShelliin
2. Suorita seuraavat komennot:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organisaation $org