---
title: Suorituskykyongelmat - SharePoint tai OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: ec378981d4f24837b037e18214cbeba2f2b657c5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692690"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="b54bb-102">SharePoint tai OneDrive Hidas, käyttökelvin tai ei käytettävissä useille käyttäjille</span><span class="sxs-lookup"><span data-stu-id="b54bb-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="b54bb-103">Jos OneDrive- tai SharePoint-sivusto ei ole useiden käyttäjien käytettävissä aiemmin, palveluongelma saattaa olla tilapäinen.</span><span class="sxs-lookup"><span data-stu-id="b54bb-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="b54bb-104">[Tarkista palvelun kunnon koontinäyttö](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="b54bb-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="b54bb-105">**Käyttäjän lisääminen ja lisensointi**</span><span class="sxs-lookup"><span data-stu-id="b54bb-105">**Add and license the user**</span></span>

<span data-ttu-id="b54bb-106">Varmista, että [määrität käyttöoikeudet Microsoft 365 for Business -järjestelmän käyttäjille.](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)</span><span class="sxs-lookup"><span data-stu-id="b54bb-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="b54bb-107">**Käyttöoikeuksien määrittäminen**</span><span class="sxs-lookup"><span data-stu-id="b54bb-107">**Assign Permissions**</span></span>

<span data-ttu-id="b54bb-108">Jos käyttäjälle on määritetty Sharepoint-käyttöoikeus ja hän saa edelleen käyttöestettyä viestiä, varmista, että hänelle on määritetty [asianmukainen käyttöoikeustaso.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="b54bb-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="b54bb-109">**Harkitse käyttöpyyntötoiminnon käyttämistä**</span><span class="sxs-lookup"><span data-stu-id="b54bb-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="b54bb-110">[Käyttöoikeuspyyntöominaisuuden](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) avulla käyttäjät voivat pyytää pääsyä sisältöön, jota heillä ei ole tällä hetkellä oikeus nähdä.</span><span class="sxs-lookup"><span data-stu-id="b54bb-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="b54bb-111">**Mukautetun komentosarjan salliminen saattaa aiheuttaa käyttöestettyjen ongelmien käytön**</span><span class="sxs-lookup"><span data-stu-id="b54bb-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="b54bb-112">On tilanteita, joissa *Salli mukautettu komentosarja* -ominaisuus saattaa estää käyttöoikeuden.</span><span class="sxs-lookup"><span data-stu-id="b54bb-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="b54bb-113">Luettelo ominaisuuksista, joita haavoittuvuus koskee, tietoturvaan liittyvistä seikoista ja mahdollisuudesta poistaa ominaisuus käytöstä.</span><span class="sxs-lookup"><span data-stu-id="b54bb-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="b54bb-114">Siirry [kohtaan Salli tai estä mukautettu komentosarja](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="b54bb-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

