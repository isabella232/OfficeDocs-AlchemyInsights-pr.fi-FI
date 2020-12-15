---
title: Google Chromen laajennukset Microsoft Edgeen (kromi)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677881"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="40182-102">Google Chromen laajennukset Microsoft Edgeen (kromi)</span><span class="sxs-lookup"><span data-stu-id="40182-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="40182-103">[Google Chromen laajennuksia on helppo käyttää Microsoft Edgeen (kromi)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span><span class="sxs-lookup"><span data-stu-id="40182-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="40182-104">Useimmissa tapa uksissa tarvitset vain vähäisiä muutoksia, jotta voit suorittaa nämä laajennukset Microsoft Edgessä.</span><span class="sxs-lookup"><span data-stu-id="40182-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="40182-105">Google Chromen tukemat laajennus ohjelmointi raja pinnat ja manifesti ovat yhteensopivia Microsoft Edgen kanssa.</span><span class="sxs-lookup"><span data-stu-id="40182-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="40182-106">Microsoft Edge ei kuitenkaan tue laajennus ohjelmointi raja pintoja Chrome. GCM, Chrome. Identity. getAccounts, Chrome. Identity. Getauthtunnus ja Chrome. instanceID.</span><span class="sxs-lookup"><span data-stu-id="40182-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>