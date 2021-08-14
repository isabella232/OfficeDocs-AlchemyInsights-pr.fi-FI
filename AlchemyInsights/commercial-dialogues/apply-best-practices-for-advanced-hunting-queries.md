---
title: Parhaiden käytäntöjen käyttäminen tarkennemmille hakukyselyille
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930130"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Parhaiden käytäntöjen käyttäminen tarkennemmille hakukyselyille

Voit saada tulokset nopeammin ja välttää aikakatkaisut monimutkaisia kyselyjä suorittamalla seuraavia parhaita käytäntöjä:

- Kun yrität uusia kyselyjä, käytä aina rajaa, jotta et saa erittäin suuria tulosjoukkoja. Käytä myös tulosjoukon koon `count` alkuarviointia.
- Käytä ensin aikasuodattimia. Ihanne parasta on rajoittaa kyselyt seitsemään päivään.
- Lisää kyselyn alkuun heti aikasuodattimen jälkeen suodattimet, jotka todennäköisesti poistavat suurimman osan tiedoista.
- Kun etsit kokonaisia tunnuksia, käytä `has` operaattoria `contains` .
- Suorita haku tietystä sarakkeesta kaikkien sarakkeiden sijaan.
- Kun liität taulukoita, määritä ensin taulukko, jossa on vähemmän rivejä.
- `project` vain tarvittavat sarakkeet taulukoista, jotka olet yhdistänyt.

Lisätietoja on kohdassa Edistyneet [hakukyselyn parhaat käytännöt.](https://go.microsoft.com/fwlink/?linkid=2144812)
