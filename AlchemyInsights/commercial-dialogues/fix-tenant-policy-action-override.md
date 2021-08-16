---
title: Korjaa vuokraajakäytäntö (toiminnon ohittaminen)
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
ms.openlocfilehash: 9c0b88c1ca2120acccd9cd75eb918a81bde52ec3919f6148922f077f07899da7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034931"
---
# <a name="fix-tenant-policy-action-override"></a>Korjaa vuokraajakäytäntö (toiminnon ohittaminen)

Viesti vaikuttaa vuokraajan roskapostin estokäytäntöön. Voit tarkistaa käytännön seuraavasti:

1. Siirry Office 365 [tietoturva- & yhteensopivuuskeskukseen](https://go.microsoft.com/fwlink/p/?linkid=2077143)ja siirry sitten Threat Management Policy Anti-spam (Uhkien   >  **hallintakäytäntö**  >  [roskapostin esto) -keskukseen.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Tarkista, onko **käytäntölähde** merkkinä seuraavasta:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC (Lisää-Xheader/ModifySubject/Redirect/Delete/No action/ BCC)**

    Jos näin on, **tarkista Mukautettu-välilehdessä** sen käytännön asetukset, johon viesti vaikuttaa. On mahdollista, että **vakioasetuksia sovelletaan kaikkiin** Exchange Online Protection vaikuttaa viestiin.

Lisätietoja roskapostin suodatuskäytäntöjen määrittämisestä on kohdassa [Roskapostin suodatuskäytäntöjen määrittäminen.](https://go.microsoft.com/fwlink/?linkid=2101431)
