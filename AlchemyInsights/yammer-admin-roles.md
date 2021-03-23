---
title: Tietoja Yammer järjestelmänvalvojille
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/22/2021
ms.locfileid: "51036720"
---
# <a name="about-yammer-admins"></a><span data-ttu-id="ecb6f-102">Tietoja Yammer järjestelmänvalvojille</span><span class="sxs-lookup"><span data-stu-id="ecb6f-102">About Yammer admins</span></span>

<span data-ttu-id="ecb6f-103">**Verkoston järjestelmänvalvojat**</span><span class="sxs-lookup"><span data-stu-id="ecb6f-103">**Network admins**</span></span>

<span data-ttu-id="ecb6f-104">Yleiset järjestelmänvalvojat ylentyvät automaattisesti varmennetuksi järjestelmänvalvojan rooliksi Yammer verkostossa.</span><span class="sxs-lookup"><span data-stu-id="ecb6f-104">Global admins are automatically promoted to the Verified Admin role in a Yammer network.</span></span> <span data-ttu-id="ecb6f-105">Seuraavissa tapauksissa tämä kampanja ei ehkä tapahdu oikein:</span><span class="sxs-lookup"><span data-stu-id="ecb6f-105">In the following cases, this promotion may not occur correctly:</span></span>

- <span data-ttu-id="ecb6f-106">Useita Yammer on olemassa, ja järjestelmänvalvoja on kirjautuneena väärään verkostoon.</span><span class="sxs-lookup"><span data-stu-id="ecb6f-106">Multiple Yammer networks exist, and the admin is being signed into the wrong one.</span></span> <span data-ttu-id="ecb6f-107">[Verkon yhdistäminen](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) on tarpeen, jotta voit käyttää Yammer verkostoa.</span><span class="sxs-lookup"><span data-stu-id="ecb6f-107">[Network consolidation](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is required to get to one Yammer network.</span></span>
- <span data-ttu-id="ecb6f-108">Azure PIM:iä käytetään.</span><span class="sxs-lookup"><span data-stu-id="ecb6f-108">Azure PIM is being used.</span></span> <span data-ttu-id="ecb6f-109">Käyttäjää ei ehkä ylennetä yleisvalvojaksi niin kauan, että kampanja voidaan tehdä.</span><span class="sxs-lookup"><span data-stu-id="ecb6f-109">The user may not be promoted to global admin long enough for the promotion to occur.</span></span> <span data-ttu-id="ecb6f-110">Tuleva päivitys Yammer ratkaista ongelman, mutta käyttäjien on parasta ylentää käyttäjiä yleisiin järjestelmänvalvojiin manuaalisesti.</span><span class="sxs-lookup"><span data-stu-id="ecb6f-110">A future update to Yammer may resolve this issue, but it is best to promote users to global admin manually.</span></span>
- <span data-ttu-id="ecb6f-111">Synkronointiongelma on olemassa Yammer kanssa.</span><span class="sxs-lookup"><span data-stu-id="ecb6f-111">A sync issue exists with the Yammer network.</span></span> <span data-ttu-id="ecb6f-112">Tässä tapauksessa lisätutkimusta varten tarvitaan tukipyyntö.</span><span class="sxs-lookup"><span data-stu-id="ecb6f-112">In this case a support request will be required for further investigation.</span></span>

<span data-ttu-id="ecb6f-113">Lisätietoja järjestelmänvalvojan Yammer on kohdassa [Järjestelmänvalvojien Yammer hallinta.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins)</span><span class="sxs-lookup"><span data-stu-id="ecb6f-113">For more information about Yammer admin roles, see [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span></span>

<span data-ttu-id="ecb6f-114">**Ryhmän järjestelmänvalvojat**</span><span class="sxs-lookup"><span data-stu-id="ecb6f-114">**Group admins**</span></span>

<span data-ttu-id="ecb6f-115">Microsoft 365:ssä yhdistettyjen ryhmien ryhmän järjestelmänvalvojat synkronoidaan Azure AD:n ryhmän jäsenyyksien kanssa.</span><span class="sxs-lookup"><span data-stu-id="ecb6f-115">Group admins for Microsoft 365 connected groups are synced with group membership from Azure AD.</span></span> <span data-ttu-id="ecb6f-116">Suurissa ryhmissä synkronointi voi kestää pitkään.</span><span class="sxs-lookup"><span data-stu-id="ecb6f-116">For large groups, this sync can take an extended period.</span></span>
