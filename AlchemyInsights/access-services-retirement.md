---
title: Access services-eläke
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973914"
---
# <a name="access-services-retirement"></a><span data-ttu-id="8fd9f-102">Access services-eläke</span><span class="sxs-lookup"><span data-stu-id="8fd9f-102">Access services retirement</span></span>

<span data-ttu-id="8fd9f-103">Olemme alun perin ilmoitti maaliskuuta 2017-MC97576, ja jatkoi kommunikoida kuluneen vuoden aikana Access Services ovat parhaillaan aktiivisesta Office 365: ssä.</span><span class="sxs-lookup"><span data-stu-id="8fd9f-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="8fd9f-104">Tämän prosessin seuraava vaihe on käyttää WWW-tietokantoja, jotka käyttävät SharePoint-luetteloita niiden pohjana olevat tiedot varastona poistamista.</span><span class="sxs-lookup"><span data-stu-id="8fd9f-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

## <a name="how-does-this-affect-me"></a><span data-ttu-id="8fd9f-105">Miten tämä vaikuttaa minulle?</span><span class="sxs-lookup"><span data-stu-id="8fd9f-105">How does this affect me?</span></span>

<span data-ttu-id="8fd9f-106">Kesäkuuta 2019 alkaen olemme lopettaa SharePoint Onlinen uusien Access-tietokantojen perustamista ja sammuttaa palvelu ja kaikki muut apps huhtikuu vuoteen 2020 mennessä.</span><span class="sxs-lookup"><span data-stu-id="8fd9f-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a><span data-ttu-id="8fd9f-107">Mitä pitää tehdä tämän muutoksen valmistautua?</span><span class="sxs-lookup"><span data-stu-id="8fd9f-107">What do I need to do to prepare for this change?</span></span>

<span data-ttu-id="8fd9f-108">Kehotamme luomaan organisaation Access-web-tietokantojen siirtyminen suunnitelma.</span><span class="sxs-lookup"><span data-stu-id="8fd9f-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="8fd9f-109">Valvojat hankkia Access-sovellukset, jotka käyttävät sivustot luettelo [SharePoint käyttää app skannerin](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) avulla.</span><span class="sxs-lookup"><span data-stu-id="8fd9f-109">Admins can use the [SharePoint Access app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="8fd9f-110">Access web-tietokantojen tietojen siirtäminen seuraavilla tavoilla:</span><span class="sxs-lookup"><span data-stu-id="8fd9f-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="8fd9f-111">Tuodaan paikallinen Access-tietokanta (. ACCDB) tai Excel-tiedostoon.</span><span class="sxs-lookup"><span data-stu-id="8fd9f-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="8fd9f-112">Suosittelemme myös interaktiiviseen Microsoft PowerApps kuin vaihtoehtoinen ympäristössä kooditon mukautettujen ratkaisujen luominen web ja mobiililaitteet.</span><span class="sxs-lookup"><span data-stu-id="8fd9f-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>