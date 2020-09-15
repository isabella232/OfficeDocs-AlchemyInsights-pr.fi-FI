---
title: Sisältö haku ei tulosta
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680644"
---
# <a name="no-results-from-content-searchexports"></a>Ei tuloksia sisältö hausta/viennistä

Sisältö haun ja viennin ongelmat, jotka eivät palauta mitään tietoja, voivat johtua siitä, että tietty järjestelmänvalvoja on saattanut määrittää tietyt yhteensopivuus tieto turva suodattimet eikä tiedota asiasta kaikille järjestelmänvalvojille.

Jos haluat korjata tämän ongelman, tarkista, onko yhteensopivuus suojausta mahdollisesti aiheuttava.
1. Yhteyden muodostaminen tieto turva-ja yhteensopivuus keskuksen PowerShellin avulla
2. Suorita seuraavat komentosovelmat:
<br>$org = "yourdomain.com"
<br>Get-Compreancesecurityfilter-Organization $org