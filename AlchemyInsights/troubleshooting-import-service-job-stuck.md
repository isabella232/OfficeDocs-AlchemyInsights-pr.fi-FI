---
title: Tuontipalvelutyön jumiutuessa vianmääritys
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125106"
---
# <a name="troubleshooting-import-service-job-stuck"></a>Tuontipalvelutyön jumiutuessa vianmääritys

Jos sinulla on ongelmia jumiutuvien tai epäonnistuvien tuontipalvelutöiden kanssa, tarkista ja kokeile seuraavaa:

- Tarkista PST-tiedoston koko. PST-tiedoston tuonnin suositeltu enimmäiskoko on 20 Gt.

- Jos epäilet ohittaneen kohteita vioittumisen vuoksi, suorita Scanpst.exe pst-tiedostojen virheiden vianmääritystä ja korjaamista varten.

- Jos näet Tuonnin aikana MapiExceptionTyökalutoffQuotaExceeded-virheen, varmista, että kohdepostilaatikossa on riittävästi kapasiteettia haluttujen PST-tiedostojen tuomiseen.

Lisätietoja PST-tuontityön ongelmien vianmäärityksestä on kohdassa [PST-tuontitöiden ongelmien vianmääritys.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

Lisätietoja siitä, miten voit korjata ongelmia tuotaessa PST-tiedostoja Outlook on kohdassa [.pst-tiedoston Outlook (microsoft.com) ongelmien ratkaiseminen.](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)