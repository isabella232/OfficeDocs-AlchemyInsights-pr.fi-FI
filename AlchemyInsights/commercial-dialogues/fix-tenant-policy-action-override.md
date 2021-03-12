---
title: Vuokraajan käytännön korjauksen (toiminnon ohittaminen)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745885"
---
# <a name="fix-tenant-policy-action-override"></a>Vuokraajan käytännön korjauksen (toiminnon ohittaminen)

Tämä sanoma vaikuttaa vuokraajan roskapostin estokäytäntöön. Voit tarkistaa käytännön seuraavasti:

1. Siirry [Office 365:n tietoturva- & yhteensopivuuskeskukseen](https://go.microsoft.com/fwlink/p/?linkid=2077143)ja siirry sitten **uhkien**  >  **hallintakäytäntöön**  >  [roskapostin estoon.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Tarkista, onko **käytäntölähde** ilmaise seuraavaa:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**

    Jos näin on, tarkista Mukautetut-välilehdessä sen käytännön asetukset, johon viesti vaikuttaa.  On mahdollista, että  kaikkiin Exchange Online Protection -asiakkaisiin sovellettiin vakioasetuksia, joihin viesti vaikuttaa.

Lisätietoja roskapostin suodatuskäytäntöjen määrittämisestä on kohdassa [Roskapostisuodatinkäytäntöjen määrittäminen.](https://go.microsoft.com/fwlink/?linkid=2101431)
