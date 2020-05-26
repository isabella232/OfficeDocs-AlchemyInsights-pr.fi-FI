---
title: Estä linkkien jakamisen estäminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 8cb53754125cedf4a3d0426d6c3bf70297eb3d74
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/23/2020
ms.locfileid: "44357628"
---
# <a name="block-download-on-sharing-links"></a>Estä linkkien jakamisen estäminen

**Estä lataaminen** on käytettävissä **vain katselu - linkeissä Office-asiakirjoihin.** Kun valitset tämän vaihtoehdon, käyttäjät, jotka voivat käyttää tiedostoa luomasi linkin kautta, eivät näe tiedoston lataus-, tulostus- tai kopiointiasetuksia.

Järjestelmänvalvojat voivat määrittää, näkyykö estolatausasetus vain Office-tiedostoissa vai ei, muuttamalla `BlockDownloadLinksFileType` [Set-SPOTenant-](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) tai [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell -cmdlet-komentojen asetusta.
