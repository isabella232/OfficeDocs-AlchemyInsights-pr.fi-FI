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
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627843"
---
# <a name="data-location"></a>Tietojen sijainti

Voit tarkastella Office 365-vuokra ajan sijaintia hallinta keskuksessa tai yhdistämällä Exchange Onlineen PowerShellin kautta.


**Hallinta keskus:**
1. Kirjaudu [hallinta keskukseen](https://admin.microsoft.com/Adminportal/Home).
2. Valitse **Asetukset** > -**organisaatio profiili**.
3. Valitse **tietojen sijainti**-kohdassa **Näytä tiedot**.


**Powershell:**
1. Muodosta yhteys Exchange Onlineen Windows PowerShellin avulla.
2. Suorita [Hanki-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) -cmdlet-komentoa näyttääksesi luettelon vuokra ajan ominaisuuksista. 
3. Katso OrganizationId-ominaisuutta.

Kun tieto sijainti on EXO ja SPO, voit määrittää datan sijainnin muille palveluille, joita voit käyttää [tietojen](https://products.office.com/where-is-your-data-located)sijainti paikasta.