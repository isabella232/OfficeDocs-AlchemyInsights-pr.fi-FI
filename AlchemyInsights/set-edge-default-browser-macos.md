---
title: Microsoft Edgen asetaminen oletusselaimeksi macOS-laitteessa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491552"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="d1f9a-102">Microsoft Edgen asetaminen oletusselaimeksi macOS-laitteessa</span><span class="sxs-lookup"><span data-stu-id="d1f9a-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="d1f9a-103">Määritä Microsoft Edge oletusselaimeksi jollakin seuraavista tavoista:</span><span class="sxs-lookup"><span data-stu-id="d1f9a-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="d1f9a-104">Menetelmä 1: Flash-laite, jossa on macOS-kuva, jossa Microsoft Edge on jo määritetty oletusselaimeksi.</span><span class="sxs-lookup"><span data-stu-id="d1f9a-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="d1f9a-105">Menetelmä 2: Aseta DefaultBrowserSettingEnabled-käytäntö, joka kehottaa käyttäjää asettamaan Microsoft Edgen oletusselaimeksi.</span><span class="sxs-lookup"><span data-stu-id="d1f9a-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="d1f9a-106">Kumman tahansa menetelmän avulla käyttäjä voi vaihtaa oletusselaimen.</span><span class="sxs-lookup"><span data-stu-id="d1f9a-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="d1f9a-107">Tästä syystä suosittelemme, että otat DefaultBrowserSettingEnabled-käytännön käyttöön, vaikka käytit menetelmää 1.</span><span class="sxs-lookup"><span data-stu-id="d1f9a-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="d1f9a-108">Jos käyttäjä vaihtaa oletusselaimen, kun käytäntö on otettu käyttöön, käytäntö kehottaa käyttäjää asettamaan oletusselaimen takaisin Microsoft Edgeen.</span><span class="sxs-lookup"><span data-stu-id="d1f9a-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
