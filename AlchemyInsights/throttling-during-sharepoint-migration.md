---
title: Rajoittaminen SharePoint-siirron aikana
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "9000353"
- "1987"
- "9000136"
- "2968"
ms.assetid: ''
ms.openlocfilehash: dc77c462fcf32817c92709852e2d03ab2086b9a4
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958895"
---
# <a name="sharepoint-throttling"></a><span data-ttu-id="a7a2a-102">SharePointin rajoittaminen</span><span class="sxs-lookup"><span data-stu-id="a7a2a-102">SharePoint throttling</span></span>

<span data-ttu-id="a7a2a-103">**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="a7a2a-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="a7a2a-104">**SharePoint Onlinen rajoittaminen**</span><span class="sxs-lookup"><span data-stu-id="a7a2a-104">**SharePoint Online throttling**</span></span>

<span data-ttu-id="a7a2a-105">SharePoint Online käyttää rajoittamista SharePoint Online -palvelun optimaalisen suorituskyvyn ja luotettavuuden ylläpitämiseen.</span><span class="sxs-lookup"><span data-stu-id="a7a2a-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="a7a2a-106">Rajoittaminen rajoittaa käyttäjien toimien tai samanaikaisten kutsujen määrää (komentosarjojen tai koodin avulla), jotta resurssien liikakäyttö estetään.</span><span class="sxs-lookup"><span data-stu-id="a7a2a-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span>

<span data-ttu-id="a7a2a-107">Lisätietoja saat seuraavista linkeistä:</span><span class="sxs-lookup"><span data-stu-id="a7a2a-107">For more information please visit the links below:</span></span>

- [<span data-ttu-id="a7a2a-108">Rajoittumisen tai käytön estymisen välttäminen SharePoint Onlinessa</span><span class="sxs-lookup"><span data-stu-id="a7a2a-108">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)
- [<span data-ttu-id="a7a2a-109">Tietojen siirto ja SPO:n rajoittaminen</span><span class="sxs-lookup"><span data-stu-id="a7a2a-109">Data Migration and SPO Throttling</span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)
- [<span data-ttu-id="a7a2a-110">SharePoint Onlinen ja OneDriven siirtonopeus</span><span class="sxs-lookup"><span data-stu-id="a7a2a-110">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
- [<span data-ttu-id="a7a2a-111">Hallitse SharePoint Onlinen rajoittamista eksponentiaalisen peruutuksen avulla</span><span class="sxs-lookup"><span data-stu-id="a7a2a-111">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)
- [<span data-ttu-id="a7a2a-112">Kapasiteetin suunnittelu ja kuormituksen testaus SharePoint Onlinessa</span><span class="sxs-lookup"><span data-stu-id="a7a2a-112">Capacity planning and load testing SharePoint Online</span></span>](https://support.office.com/article/Capacity-planning-and-load-testing-SharePoint-Online-c932bd9b-fb9a-47ab-a330-6979d03688c0)
- [<span data-ttu-id="a7a2a-113">Siirron aikana ilmenee suorituskyvyn heikkenemistä tai rajoittumista</span><span class="sxs-lookup"><span data-stu-id="a7a2a-113">I am experiencing poor performance or throttling during migration</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed#faq-and-troubleshooting)