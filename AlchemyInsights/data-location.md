---
title: Tietojen sijainti
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655279"
---
# <a name="data-location"></a>Tietojen sijainti

Voit tarkastella vuokraajan sijaintia hallintakeskuksessa tai muodostamalla yhteyden Exchange Onlineen PowerShellin kautta.


**Hallintakeskus:**
1. Kirjaudu [hallintakeskukseen](https://admin.microsoft.com/Adminportal/Home).
2. Valitse **Asetukset** > **Organisaatioprofiili**.
3. Valitse **Tietojen sijainti**-kohdassa Näytä **tiedot**.


**Powershell:**
1. Muodosta yhteys Exchange Onlineen Windows PowerShellin avulla.
2. Suorita [Get-OrganizationalUnit-cmdlet-komento,](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) jolloin näkyviin tulee luettelo vuokraajan ominaisuuksista. 
3. Katso OrganizationId-ominaisuutta.

Kun sinulla on EXO:n ja SPO:n tietosijainti, voit määrittää muiden palveluiden tietosijainnin, jota voit käyttää [kohdasta Missä tietosi sijaitsevat](https://products.office.com/where-is-your-data-located).