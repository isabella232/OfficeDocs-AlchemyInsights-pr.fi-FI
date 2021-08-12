---
title: 0x8004de40 käynnistäessäsi OneDrive
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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946576"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 käynnistäessäsi OneDrive

Jos saat virheilmoituksen **0x8004de40** kirjauduttaessa OneDrive, käynnistä tietokone uudelleen, kun olet yhteydessä työ- tai koulutoimialueeseen. Jos saat tämän virheen uudelleenkäynnistyksen jälkeen, kokeile tätä, kun olet muodostanut yhteyden työ- tai koulutoimialueeseen:

1. Valitse Käynnistä ja kirjoita  **hakuruutuun cmd** tai komentokehote, napsauta komentokehotesovellusta hiiren kakkospainikkeella ja valitse **Suorita järjestelmänvalvojana**. Jos sinua pyydetään antamaan järjestelmänvalvojan salasana tai vahvistus, kirjoita salasana tai valitse **Salli**.  

2. Kirjoita Komentokehote-ikkunassa **dsregcmd /leave**  ja odota, että komento on valmis. Kirjoita **sitten dsregcmd /join** ja odota, että komento on valmis.
3. Käynnistä tietokone uudelleen.
