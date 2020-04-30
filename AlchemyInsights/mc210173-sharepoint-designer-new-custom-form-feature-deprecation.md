---
title: MC210173 – SharePoint Designerin uuden mukautetun lomakeominaisuuden käytöstä poistuminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 185e8fc94345b240667490b1ffc63af8459d8daf
ms.sourcegitcommit: a9e6b2fcce8bd12fd079ed967f426b67d5c6d239
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/28/2020
ms.locfileid: "43928525"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="9d69d-102">MC210173 – SharePoint Designerin uuden mukautetun lomakeominaisuuden käytöstä poistuminen</span><span class="sxs-lookup"><span data-stu-id="9d69d-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="9d69d-103">Microsoft on tunnistanut SharePoint Designerin [mukautettujen lomakkeiden luomiseen](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) liittyvän ongelman SharePoint Onlinessa.</span><span class="sxs-lookup"><span data-stu-id="9d69d-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="9d69d-104">Huolellisen tarkastelun jälkeen Microsoft on määrittänyt, että tähän ongelmaan ei ole tunnettua korjausta, ja mukautettujen lomakkeiden luomistoiminto on päätetty poistaa käytöstä lauantaista 25.4.2020 kello 3.00 (UTC) alkaen.</span><span class="sxs-lookup"><span data-stu-id="9d69d-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="9d69d-105">Tämä muutos ei vaikuta aiemmin luotujen lomakkeiden tai muiden olemassa olevien toimintojen muokkaamiseen SharePoint Online Designerissa.</span><span class="sxs-lookup"><span data-stu-id="9d69d-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="9d69d-106">Tämän muutoksen tekemisen jälkeen käyttäjät saattoivat saada seuraavanlaisen virheilmoituksen uusia lomakkeita luodessaan: "Luettelomuutosten tallentaminen palvelimeen ei onnistunut".</span><span class="sxs-lookup"><span data-stu-id="9d69d-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="9d69d-107">Käyttäjät, jotka ovat aiemmin käyttäneet SharePoint Designeria mukautettujen lomakkeiden luomiseen, voivat nyt käyttää [PowerAppsia](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) tähän tarkoitukseen.</span><span class="sxs-lookup"><span data-stu-id="9d69d-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="9d69d-108">PowerApps on helppokäyttöinen ja tehokas työkalu, joka mahdollistaa SharePoint Online Modernin käyttäjiä luomaan ja muokkaamaan SharePoint-luetteloiden ja tiedostokirjastojen mukautettuja lomakkeita suoraan selainikkunassa.</span><span class="sxs-lookup"><span data-stu-id="9d69d-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="9d69d-109">PowerApps ei edellytä koodausosaamista tai lisäsovellusten, kuten InfoPathin, lataamista.</span><span class="sxs-lookup"><span data-stu-id="9d69d-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="9d69d-110">**Huomautus**: SharePoint Online Classicin käyttäjien on vaihdettava tilapäisesti Modern-käyttökokemukseen, jotta he voivat käyttää PowerAppsia. Kaikki PowerAppsissa luodut muokatut lomakkeet ovat kuitenkin SharePoint Online Classicin käyttäjien käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="9d69d-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
