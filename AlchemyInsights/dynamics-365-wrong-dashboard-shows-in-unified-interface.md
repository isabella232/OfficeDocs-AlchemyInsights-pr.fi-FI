---
title: Dynamics 365-Dynamics 365 Unified Interface-liittymän väärät koonti näyttöjen esitykset
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528548"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Dynamics 365 Unified Interface-liittymän väärät koonti näyttöjen esitykset

On useita syitä, miksi saatat nähdä eri koonti näytön kuin mitä odotat:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Käyttäjä on määrittänyt käyttäjän oletus koonti näytön 

Yleensä voit tunnistaa käyttäjän oletus koonti näytön, jos **Aseta oletus** arvoksi-painike ei näy koonti näytön komento palkissa. Käyttäjän oletus koonti näyttö ohittaa kaikki muut oletus koonti näytöt, vaikka käyttäjän oletus koonti näyttö ei olisi nykyisessä sovelluksessa.

Poista oletus koonti näytön asetus käytöstä seuraavan kierto tavan avulla.

1. Luo uusi henkilökohtainen koonti näyttö.

2. Määritä uusi koonti näyttö käyttäjän oletus arvoksi.

3. Poista kyseinen koonti näyttö.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Koonti näyttö on määritetty sivustokartassa

Olet ehkä määrittänyt organisaation oletus koonti näytön valitsemalla koonti näytön ja valitsemalla "Määritä oletukseksi" kohdassa "Mukauta järjestelmää". Sivustokartan suunnittelu ohjelmassa määritetty koonti näyttö ohittaa kuitenkin tämän koonti näytön, jos käyttäjällä on siihen käyttö oikeus.

Jotta käyttäjät näkevät koonti näytön, jonka olet määrittänyt organisaation oletus arvoksi, voit joko:

* Määritä tämä koonti näyttö sivustokartassa

* Poista käyttö oikeudet sivustokartan määritettyyn koonti näyttöön näille käyttäjille
