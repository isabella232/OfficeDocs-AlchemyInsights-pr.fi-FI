---
title: Rajoittaa perinteistä SharePoint Online
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: e7ecfd8c2f1a532355bfb8c2c0a846fc0d6e88b1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551556"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="46681-102">Rajoittaa perinteistä SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="46681-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="46681-103">Joissakin organisaatioissa on vielä Classic-tilassa kokemus.</span><span class="sxs-lookup"><span data-stu-id="46681-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="46681-104">Kun ei aiota poistaa porrastetusti perinteistä, ei enää voi rajoittaa koko organisaation (vuokraaja) luetteloiden ja kirjastojen perinteistä.</span><span class="sxs-lookup"><span data-stu-id="46681-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="46681-105">Admin on hallita yksittäisten luetteloiden ja kirjastojen avulla rakeinen Yllättävät valitsimia, joita annamme seuraavilla tasoilla classic-tilassa seuraavista vaihtoehdoista:</span><span class="sxs-lookup"><span data-stu-id="46681-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="46681-106">sivustokokoelman</span><span class="sxs-lookup"><span data-stu-id="46681-106">site collection</span></span>
- <span data-ttu-id="46681-107">sivuston</span><span class="sxs-lookup"><span data-stu-id="46681-107">site</span></span>
- <span data-ttu-id="46681-108">luettelo</span><span class="sxs-lookup"><span data-stu-id="46681-108">list</span></span>
- <span data-ttu-id="46681-109">kirjasto</span><span class="sxs-lookup"><span data-stu-id="46681-109">library</span></span>

<span data-ttu-id="46681-110">Lisäksi luetteloita, jotka käyttävät tiettyjä ominaisuuksia ja mukautukset, joita ei tueta Moderni edelleen olla automaattisesti siirtynyt perinteistä.</span><span class="sxs-lookup"><span data-stu-id="46681-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="46681-111">1. huhtikuuta 2019, käytöstä vuokralaisen tason prosessi alkaa Moderni luettelon säännöksen ja kirjastojen käynnistää ja jatkaa – 31. toukokuuta 2019.</span><span class="sxs-lookup"><span data-stu-id="46681-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="46681-112">Luetteloita ja kirjastoja, jotka ovat perinteistä johdosta vuokralaisen ei sisälly automaattisesti siirtää, Moderni.</span><span class="sxs-lookup"><span data-stu-id="46681-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="46681-113">Jos tarvitset perinteistä Katso lisätietoja [tähän](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) ja PnP Powershell-Ohje [tähän](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , jotka kuvaavat vaihtoehdot ja työkalujen avulla voit nyt käyttää perinteistä kokemus.</span><span class="sxs-lookup"><span data-stu-id="46681-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
