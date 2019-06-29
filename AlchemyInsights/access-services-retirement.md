---
title: Access services-eläke
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 5f171050479f34077f3dc155bec40437f86b84c0
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35359340"
---
# <a name="access-services-retirement"></a><span data-ttu-id="738cc-102">Access services-eläke</span><span class="sxs-lookup"><span data-stu-id="738cc-102">Access services retirement</span></span>

<span data-ttu-id="738cc-103">Olemme alun perin ilmoitti maaliskuuta 2017-MC97576, ja jatkoi kommunikoida kuluneen vuoden aikana Access Services ovat parhaillaan aktiivisesta Office 365: ssä.</span><span class="sxs-lookup"><span data-stu-id="738cc-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="738cc-104">Tämän prosessin seuraava vaihe on käyttää WWW-tietokantoja, jotka käyttävät SharePoint-luetteloita niiden pohjana olevat tiedot varastona poistamista.</span><span class="sxs-lookup"><span data-stu-id="738cc-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="738cc-105">**Miten tämä vaikuttaa minulle?**</span><span class="sxs-lookup"><span data-stu-id="738cc-105">**How does this affect me?**</span></span>

<span data-ttu-id="738cc-106">Kesäkuuta 2019 alkaen olemme lopettaa SharePoint Onlinen uusien Access-tietokantojen perustamista ja sammuttaa palvelu ja kaikki muut apps huhtikuu vuoteen 2020 mennessä.</span><span class="sxs-lookup"><span data-stu-id="738cc-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="738cc-107">**Mitä pitää tehdä tämän muutoksen valmistautua?**</span><span class="sxs-lookup"><span data-stu-id="738cc-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="738cc-108">Kehotamme luomaan organisaation Access-web-tietokantojen siirtyminen suunnitelma.</span><span class="sxs-lookup"><span data-stu-id="738cc-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="738cc-109">Valvojat hankkia Access-sovellukset, jotka käyttävät sivustot luettelo [SharePoint käyttää app skannerin](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) avulla.</span><span class="sxs-lookup"><span data-stu-id="738cc-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="738cc-110">Access web-tietokantojen tietojen siirtäminen seuraavilla tavoilla:</span><span class="sxs-lookup"><span data-stu-id="738cc-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="738cc-111">Tuodaan paikallinen Access-tietokanta (. ACCDB) tai Excel-tiedostoon.</span><span class="sxs-lookup"><span data-stu-id="738cc-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="738cc-112">Suosittelemme myös interaktiiviseen Microsoft PowerApps kuin vaihtoehtoinen ympäristössä kooditon mukautettujen ratkaisujen luominen web ja mobiililaitteet.</span><span class="sxs-lookup"><span data-stu-id="738cc-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>