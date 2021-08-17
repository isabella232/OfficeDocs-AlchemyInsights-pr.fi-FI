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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057999"
---
# <a name="no-results-from-content-searchexports"></a>Ei tuloksia sisältöhaun/vientien avulla

Sisältöhaun ja viennin ongelmat, jotka eivät palauta tietoja, voivat johtua tietyistä tietyn järjestelmänvalvojan määritysten yhteensopivuuden suojaussuodattimesta, joka ei ole ilmoittanut siitä kaikille järjestelmänvalvojille.

Voit ratkaista ongelman tarkistamaan, aiheuttavatko ne yhteensopivuuden suojaussuodattimet:
1. Näyttöyhteys powershellin tietoturva- ja yhteensopivuuskeskukseen
2. Suorita seuraavat komennot:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organisaation $org