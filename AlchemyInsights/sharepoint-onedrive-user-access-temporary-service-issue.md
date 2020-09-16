---
title: Suorituskyky ongelmat-SharePoint tai OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771241"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="3200c-102">SharePointin tai OneDriven hidas, saavuttamattomissa tai poissa käytöstä useille käyttäjille</span><span class="sxs-lookup"><span data-stu-id="3200c-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="3200c-103">Jos OneDrive-tai SharePoint-sivusto ei ole käytettävissä useille käyttäjille, joilla on aiemmin ollut käyttö oikeus, kyseessä saattaa olla väliaikainen palvelu ongelma.</span><span class="sxs-lookup"><span data-stu-id="3200c-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="3200c-104">[Tarkista palvelun kunnon koonti näyttö](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="3200c-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="3200c-105">**Käyttäjän lisääminen ja käyttö oikeuksien määrittäminen**</span><span class="sxs-lookup"><span data-stu-id="3200c-105">**Add and license the user**</span></span>

<span data-ttu-id="3200c-106">Varmista, että määrität [käyttäjille käyttö oikeudet Microsoft 365 for Businessissa](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="3200c-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="3200c-107">**Käyttö oikeuksien määrittäminen**</span><span class="sxs-lookup"><span data-stu-id="3200c-107">**Assign Permissions**</span></span>

<span data-ttu-id="3200c-108">Jos käyttäjälle on määritetty SharePoint-käyttö oikeus ja saat edelleen käyttö estetty-viestin, varmista, että hänelle on määritetty [tarvittava käyttö oikeus taso](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="3200c-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="3200c-109">**Käyttö oikeus pyyntö toiminnon käyttäminen**</span><span class="sxs-lookup"><span data-stu-id="3200c-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="3200c-110">[Käyttö oikeus pyyntö-toiminnon](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) avulla käyttäjät voivat pyytää käyttö oikeutta sisältöön, jota heillä ei tällä hetkellä ole oikeus nähdä.</span><span class="sxs-lookup"><span data-stu-id="3200c-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="3200c-111">**Salli mukautettu komento sarja voi aiheuttaa käyttö estetty-ongelmia**</span><span class="sxs-lookup"><span data-stu-id="3200c-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="3200c-112">On olemassa tiettyjä tilanteita, joissa *Salli mukautettu komento sarja* -ominaisuus voi esittää käyttö estetty-toiminnon.</span><span class="sxs-lookup"><span data-stu-id="3200c-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="3200c-113">Luettelo ominaisuuksista, joihin ongelma vaikuttaa, tieto turvaan liittyviä seikkoja ja mahdollisuus poistaa ominaisuus käytöstä.</span><span class="sxs-lookup"><span data-stu-id="3200c-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="3200c-114">Tutustu [Salli-tai estä mukautettua komento sarjaa](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="3200c-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

