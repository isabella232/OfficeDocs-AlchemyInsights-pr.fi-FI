---
title: Sisältö haun/viennin aikana ei palautettu tuloksia
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727220"
---
# <a name="no-results-returned-during-content-searchexport"></a>Sisältö haun/viennin aikana ei palautettu tuloksia

Jos kohtaat ongelmia seuraavissa eDiscoveryn skenaarioissa:

- Sisältö haku/vienti palauttaa tietoja tai odottamattomia tietoja
- eDiscoveryn haku tai vienti epäonnistuu

Tämä voi johtua joistakin vaatimustenmukaisuutta koskevista tieto turva suodattimista, jotka on määritetty tietyn järjestelmänvalvojan toimesta ja joita ei ole toimitettu kaikille järjestelmänvalvojille.

Jos haluat korjata ongelman, tarkista, että seuraavat ongelmat voivat aiheuttaa yhteensopivuus suojausta:

1. Yhteyden muodostaminen tieto turva-ja yhteensopivuus keskuksen PowerShellin avulla
2. Suorita seuraavat komentosovelmat:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Lisä tietoja yhteensopivuuden suojaus suodattimista on Ohje aiheessa [sisältö haun käyttö oikeuksien suodattaminen](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
