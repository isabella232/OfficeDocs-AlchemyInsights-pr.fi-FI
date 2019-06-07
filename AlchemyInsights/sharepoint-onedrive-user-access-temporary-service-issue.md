---
title: Suorituskyvyn ongelmat-SharePoint- tai OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 745a62c917c0b94501843332d70609261c6d3b76
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34759148"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="90eef-102">SharePoint- tai OneDrive on hidas tai ei voi käyttää useita käyttäjiä</span><span class="sxs-lookup"><span data-stu-id="90eef-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="90eef-103">Jos OneDrive tai SharePoint-sivustossa ei ole aikaisemmin olleet tekemisissä useiden käyttäjien käytettävissä, saattaa olla väliaikaista palvelua ongelma.</span><span class="sxs-lookup"><span data-stu-id="90eef-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="90eef-104">[Tarkista palvelun terveyden dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="90eef-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="90eef-105">Lisää ja anna käyttäjän</span><span class="sxs-lookup"><span data-stu-id="90eef-105">Add and license the user</span></span>

<span data-ttu-id="90eef-106">Varmista, että voit [määrittää käyttöoikeuksia käyttäjille Office 365 yrityksille](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="90eef-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="90eef-107">**Käyttöoikeuksien määrittäminen**</span><span class="sxs-lookup"><span data-stu-id="90eef-107">**Assign Permissions**</span></span>

<span data-ttu-id="90eef-108">Jos käyttäjä on määritetty Sharepoint-käyttöoikeus ja silti saa käyttö estetty-sanoman, varmista, että ne on määritetty [asianmukaisen käyttöoikeustason](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="90eef-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="90eef-109">**Harkitse access request-toiminnolla**</span><span class="sxs-lookup"><span data-stu-id="90eef-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="90eef-110">[Access request-ominaisuus](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) sallii käyttäjät voivat käyttää sisältöä, joka ei tällä hetkellä heillä on oikeus pyytää.</span><span class="sxs-lookup"><span data-stu-id="90eef-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="90eef-111">**Salli mukautetun komentosarjan voi aiheuttaa ongelmia ei ole käyttöoikeutta**</span><span class="sxs-lookup"><span data-stu-id="90eef-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="90eef-112">On tiettyjä tilanteita, jossa *Salli mukautetun komentosarjan* ominaisuus voi olla esittämisen käyttö estetty.</span><span class="sxs-lookup"><span data-stu-id="90eef-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="90eef-113">Seuraavat ominaisuudet muuttuvat, luettelo, tietojen suojaus ja ominaisuus poistetaan käytöstä.</span><span class="sxs-lookup"><span data-stu-id="90eef-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="90eef-114">Vieraile osoitteessa [Salli tai estä mukautetun komentosarjan](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="90eef-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

