---
title: PST-tiedostojen tuontiongelmien vianmääritys
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826160"
---
# <a name="troubleshooting-pst-import-issues"></a>PST-tiedostojen tuontiongelmien vianmääritys

- Jos tuot tietoja Outlook-asiakasohjelmassa, katso artikkeli [Outlookin .pst-tiedoston tuomiseen liittyvien ongelmien korjaaminen](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Jos käytät tuontipalvelua ja se jumittuu, huomioi, että jokaisen Azure-tallennussijaintiin ladattavan PST-tiedoston koko saa olla enintään 20 Gt. Yli 20 Gt:n PST-tiedostot voivat vaikuttaa PST-tuontiprosessin suorituskykyyn.

- Jos haluat tarkistaa tietyn tuontityön tilan, voit käyttää [Get-MailboxImportRequest -eränimeä](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Jos haluat lukea tarkempia tietoja tuontipalvelusta, katso artikkeli [Yleiskatsaus organisaation PST-tiedostojen tuonnista](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
