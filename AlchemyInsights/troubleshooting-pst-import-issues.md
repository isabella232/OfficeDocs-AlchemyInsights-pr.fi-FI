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
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059812"
---
# <a name="troubleshooting-pst-import-issues"></a>PST-tiedostojen tuontiongelmien vianmääritys

- Jos tuot tietoja Outlookin asiakasohjelmassa, katso Outlookin [.pst-tiedoston](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)tuomiseen liittyviä ongelmia.

- Jos käytät tuontipalvelua ja se jumittuu, huomaa, että jokaisen Azure-tallennussijaintiin ladattavan PST-tiedoston koko ei saa olla yli 20 Gt. YLI 20 Gt:n PST-tiedostot voivat vaikuttaa PST-tuontiprosessin suorituskykyyn. Lisätietoja jumittuvien töiden vianmäärityksestä on kohdassa [PST-tuontitöihin vaikuttavat ongelmat.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

- Jos haluat tarkistaa tietyn tuontityön tilan, käytä [get-mailboxImportRequest -batchname.](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)

- Lisätietoja tuontipalvelusta on kohdassa Yleiskatsaus organisaation [PST-tiedostojen tuomiseen.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
