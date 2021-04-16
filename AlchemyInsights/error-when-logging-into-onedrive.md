---
title: 0x8004de40 OneDriven käynnistämisen virhesanoma
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813649"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 OneDriven käynnistämisen virhesanoma

Jos saat virheilmoituksen **0x8004de40** kirjauduttaessa OneDriveen, käynnistä tietokone uudelleen, kun olet yhteydessä työ- tai koulutoimialueeseen. Jos saat tämän virheen uudelleenkäynnistyksen jälkeen, kokeile tätä, kun olet muodostanut yhteyden työ- tai koulutoimialueeseen:

1. Valitse Käynnistä ja kirjoita  **hakuruutuun cmd** tai komentokehote, napsauta komentokehotesovellusta hiiren kakkospainikkeella ja valitse **Suorita järjestelmänvalvojana**. Jos sinua pyydetään antamaan järjestelmänvalvojan salasana tai vahvistus, kirjoita salasana tai valitse **Salli**.  

2. Kirjoita Komentokehote-ikkunassa **dsregcmd /leave**  ja odota, että komento on valmis. Kirjoita **sitten dsregcmd /join** ja odota, että komento on valmis.
3. Käynnistä tietokone uudelleen.
