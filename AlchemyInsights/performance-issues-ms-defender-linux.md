---
title: Suorituskykyongelmat Microsoft Defender for Endpointissa Linuxissa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793758"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Suorituskykyongelmat Microsoft Defender for Endpointissa Linuxissa

Tässä artikkelissa on ohjeet Microsoft Defender for Endpointin suorituskykyongelman tunnistamiseen Linuxissa.

On tärkeää ensin varmistaa, että ongelma on ratkaistu uusimmalla [versiolla](/microsoft-365/security/defender-endpoint/linux-whatsnew). 

Aloita tutkimus tutustumaan ohjeisiin, joissa [käsitellään Microsoft Defender for Endpointin suorituskykyongelmien vianmääritys Linuxissa.](/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>Poikkeukset

Poikkeukset voivat auttaa lieventämään suorituskykyongelmia. Tarkista poikkeukset ennen aloittamista, jotta mahdolliset lisäriskit ovat tiedossa ja dokumentoitu.

Lisätietoja on kohdassa [Microsoft Defender for Endpointin](/microsoft-365/security/defender-endpoint/linux-exclusions)poikkeusten määrittäminen ja vahvistaminen Linuxissa.

Jos sinulla on useita tiedostoja & pois jätettäväksi ja ne kaikki ovat samassa päätepisteessä, voi olla helpompaa jättää päätepiste pois. Helmikuun julkaisusta 101.22.80 alkaen voit jättää pois kokonaisen päätepisteen.

Jos esimerkiksi /mnt/backup on mountpoint, voit lisätä /mnt/backup poissulkevien luetteloon suorittamalla tämän komennon:

`$ mdatp exclusion folder add –path /mnt/backup`

**Huomautus:** Ohittamisen lisääminen lisää riskiä, että haittaohjelmia ei havaita ja että se on käsiteltävä ja otettava käyttöön huolellisesti.

## <a name="need-help"></a>Tarvitsetko apua?

Voit auttaa sinua tehokkaimmalla tavalla keräämalla diagnostiikkatiedot ennen tukitapauksen avaamista.
