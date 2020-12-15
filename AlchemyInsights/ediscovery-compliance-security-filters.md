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
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678676"
---
# <a name="no-results-returned-during-content-searchexport"></a>Sisältö haun/viennin aikana ei palautettu tuloksia

Jos kohtaat ongelmia seuraavissa eDiscoveryn skenaarioissa:

- Sisältö haku/vienti palauttaa tietoja tai odottamattomia tietoja
- eDiscoveryn haku tai vienti epäonnistuu

Tämä voi johtua siitä, että tietty järjestelmänvalvoja on saattanut määrittää tietyt yhteensopivuuden tieto turva suodattimen, eikä sitä ole toimitettu kaikille järjestelmänvalvojille.

Jos haluat korjata ongelman, tarkista, että seuraavat ongelmat voivat aiheuttaa yhteensopivuus suojausta:

1. Yhteyden muodostaminen tieto turva-ja yhteensopivuus keskuksen PowerShellin avulla
2. Suorita seuraavat komentosovelmat:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Lisä tietoja yhteensopivuuden suojaus suodattimista on Ohje aiheessa [sisältö haun käyttö oikeuksien suodattaminen](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
