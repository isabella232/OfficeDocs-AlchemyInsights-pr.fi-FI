---
title: Portaalista puuttuvat määritystenhallinnan laitteet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 7a11ad3c6970be2c52a7cf0696bd3810b9bd665a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789899"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="e4d9b-102">Portaalista puuttuvat määritystenhallinnan laitteet</span><span class="sxs-lookup"><span data-stu-id="e4d9b-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="e4d9b-103">Jotta laitesynkronointi toimisi, [tarvittavien Internet-päätepisteiden](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) on oltava tavoitettavissa paikallisesta palvelimesta, joka isännöi palvelun yhteyspisteroolia.</span><span class="sxs-lookup"><span data-stu-id="e4d9b-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="e4d9b-104">Katso laitesynkronoinnin vianmääritystietoja palvelun yhteyspisteessä olevasta **CMGatewaySyncUploadWorker.log**-tiedostosta.</span><span class="sxs-lookup"><span data-stu-id="e4d9b-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="e4d9b-105">Lue lisätietoja artikkelista [Vuokraajan kiinnittäminen Microsoftin päätepisteen hallinnassa](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="e4d9b-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
