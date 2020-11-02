---
title: 0x8004de40-Virhe käynnistettäessä OneDrivea
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823047"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40-Virhe käynnistettäessä OneDrivea

Jos näyttöön tulee virhe **0x8004de40,** kun kirja Udut sisään OneDriveen, Käynnistä tieto kone uudelleen, kun olet muodostanut yhteyden työpaikan tai oppi laitoksen toimi alueeseen. Jos saat tämän virheen uudelleenkäynnistyksen jälkeen, kokeile tätä, kun olet muodostanut yhteyden työpaikan tai oppi laitoksen toimi alueeseen:

1. Napsauta Käynnistä-painiketta ja kirjoita haku ruutuun **cmd** tai **komento kehote**  , napsauta komento kehote-sovellusta hiiren kakkos painikkeella ja valitse  **Suorita järjestelmänvalvojana** . Jos sinua pyydetään antamaan järjestelmänvalvojan sala sana tai vahvistamaan toiminto, kirjoita sala sana tai valitse **Salli** .  

2. Kirjoita komento kehote ikkunaan **dsregcmd/Leave**  ja odota, kunnes komento on valmis. Kirjoita sitten **dsregcmd/Join** ja odota, kunnes komento on valmis.
3. Käynnistä tieto kone uudelleen.
