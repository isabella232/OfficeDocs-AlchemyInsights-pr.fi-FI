---
title: Tuloksia ei palauteta sisältöhaun/viennin aikana
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
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101263"
---
# <a name="no-results-returned-during-content-searchexport"></a>Tuloksia ei palauteta sisältöhaun/viennin aikana

Jos sinulla on ongelmia seuraavien eDiscovery-skenaarioiden kanssa:

- Sisältöhaku ja -vienti ei tuo mitään tietoja tai odottamattomia tietoja
- eDiscovery-haku tai vienti epäonnistuu

Tämä voi johtua tietyistä yhteensopivuuden suojaussuodattimista, jotka tietty järjestelmänvalvoja on ottanut käyttöön, ja joista ei ole ilmoitettu kaikille järjestelmänvalvojille.

Voit ratkaista ongelman tarkistamaan, aiheuttavatko yhteensopivuuden suojaussuodattimet seuraavia ongelmia:

1. Näyttöyhteys powershellin tietoturva- ja yhteensopivuuskeskukseen
2. Suorita seuraavat komennot:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Lisätietoja yhteensopivuuden suojaussuodattimista on kohdassa [Sisältöhaun käyttöoikeuksien suodatus](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
