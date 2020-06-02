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
ms.openlocfilehash: 2dc0cd5f1641298853443d364eb9434ec1d9cd5a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511145"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="e3ea2-102">SharePoint tai OneDrive hidas, käyttökelvoton tai ei käytettävissä useille käyttäjille</span><span class="sxs-lookup"><span data-stu-id="e3ea2-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="e3ea2-103">Jos OneDrive- tai SharePoint-sivusto ei ole käytettävissä useille käyttäjille, joilla on aiemmin ollut käyttöoikeus, kyseessä voi olla tilapäinen palveluongelma.</span><span class="sxs-lookup"><span data-stu-id="e3ea2-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="e3ea2-104">[Tarkista palvelun kunnon koontinäyttö](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="e3ea2-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="e3ea2-105">**Käyttäjän lisääminen ja lisensoiminen**</span><span class="sxs-lookup"><span data-stu-id="e3ea2-105">**Add and license the user**</span></span>

<span data-ttu-id="e3ea2-106">Varmista, että [määrität käyttöoikeudet Microsoft 365 for Businessin käyttäjille.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="e3ea2-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="e3ea2-107">**Käyttöoikeuksien määrittäminen**</span><span class="sxs-lookup"><span data-stu-id="e3ea2-107">**Assign Permissions**</span></span>

<span data-ttu-id="e3ea2-108">Jos käyttäjälle on määritetty Sharepoint-käyttöoikeus ja hän saa edelleen käyttöestettyä sanomaa, varmista, että hänelle on määritetty [asianmukainen käyttöoikeustaso.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="e3ea2-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="e3ea2-109">**Harkitse käyttöoikeuspyyntötoiminnon käyttämistä**</span><span class="sxs-lookup"><span data-stu-id="e3ea2-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="e3ea2-110">[Käyttöoikeuspyyntöominaisuuden](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) avulla käyttäjät voivat pyytää pääsyä sisältöön, jota heillä ei ole tällä hetkellä näköoikeuksia.</span><span class="sxs-lookup"><span data-stu-id="e3ea2-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="e3ea2-111">**Salli mukautettu komentosarja saattaa aiheuttaa käyttöestettyjä ongelmia**</span><span class="sxs-lookup"><span data-stu-id="e3ea2-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="e3ea2-112">On tiettyjä tilanteita, joissa *Salli mukautettu komentosarja* -ominaisuus saattaa esittää käyttö estettyä.</span><span class="sxs-lookup"><span data-stu-id="e3ea2-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="e3ea2-113">Saat luettelon ominaisuuksista, joita haavoittuvuus koskee, tietoturvaan liittyvistä syistä ja ominaisuuden poistamisen käytöstä.</span><span class="sxs-lookup"><span data-stu-id="e3ea2-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="e3ea2-114">Siirry [kohtaan Mukautetun komentosarjan salliminen tai estäminen](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="e3ea2-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

