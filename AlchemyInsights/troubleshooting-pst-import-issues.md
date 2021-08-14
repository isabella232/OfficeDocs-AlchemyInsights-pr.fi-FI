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
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972416"
---
# <a name="troubleshooting-pst-import-issues"></a>PST-tiedostojen tuontiongelmien vianmääritys

- Jos tuot tietoja itse Outlook asiakasohjelmassa, katso [.pst-tiedoston Outlook ongelmien ratkaiseminen.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)

- Jos käytät tuontipalvelua ja se jumittuu, huomaa, että jokaisen palvelimeen ladattavan PST-tiedoston Azure-tallennus saa olla enintään 20 Gt. YLI 20 Gt:n PST-tiedostot voivat vaikuttaa PST-tuontiprosessin suorituskykyyn. Lisätietoja jumittuvien töiden vianmäärityksestä on kohdassa [PST-tuontitöihin vaikuttavat ongelmat.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

- Jos haluat tarkistaa tietyn tuontityön tilan, käytä [get-mailboxImportRequest -batchname.](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)

- Lisätietoja tuontipalvelusta on kohdassa Yleiskatsaus organisaation [PST-tiedostojen tuomiseen.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
