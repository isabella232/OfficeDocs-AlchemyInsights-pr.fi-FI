---
title: Dynamics 365 - Dynamics 365 yhtenäinen käyttöliittymä näkyy väärä Dashboard
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747499"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Dynamics 365 yhtenäinen käyttöliittymä näkyy väärä dashboard

On useita syitä, miksi saatat nähdä eri dashboard kuin sen pitääkin:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Käyttäjä on määrittänyt käyttäjän oletuskoontinäytön 

Voit yleensä tunnistaa käyttäjän oletuskoontinäytön on asetettu, jos **Aseta oletukseksi** -painike ei näy dashboard komentopalkki. Käyttäjän oletuskoontinäytön ohittaa kaikki muut oletusarvon raporttinäkymät, vaikka nykyinen app ei ole käyttäjän oletuskoontinäytön.

Käytä seuraavaa kiertotapaa, poista niiden oletuskoontinäytöksi.

1. Luo uusi oma dashboard.

2. Määrittää, että uusi dashboard käyttäjä.

3. Poista tämä koontinäyttö.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Raporttinäkymät on asetettu SiteMap

Olet ehkä määrittänyt dashboard valitsemalla ja valitsemalla ”Aseta oletukseksi” mukauttaminen järjestelmässä organisaation oletuskoontinäytöksi. Mutta määritelty sivustokartan suunnittelija dashboard ohittavat tämän koontinäytön, jos käyttäjällä on oikeus käyttää sitä.

Jos haluat nähdä raporttinäkymät, jotka olet määrittänyt oletusarvon mukaan organisaation käyttäjille, voit joko:

* Määritä tämä koontinäyttö SiteMap

* Käyttäjille käyttöoikeudet määritetty sivustokartan koontinäytön poistaminen
