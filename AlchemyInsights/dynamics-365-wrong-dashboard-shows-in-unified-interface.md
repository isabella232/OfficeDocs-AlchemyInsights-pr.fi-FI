---
title: Dynamics 365 - Dynamics 365 yhtenäinen käyttöliittymä näkyy väärä Dashboard
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747499"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="90235-102">Dynamics 365 yhtenäinen käyttöliittymä näkyy väärä dashboard</span><span class="sxs-lookup"><span data-stu-id="90235-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="90235-103">On useita syitä, miksi saatat nähdä eri dashboard kuin sen pitääkin:</span><span class="sxs-lookup"><span data-stu-id="90235-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="90235-104">Käyttäjä on määrittänyt käyttäjän oletuskoontinäytön</span><span class="sxs-lookup"><span data-stu-id="90235-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="90235-105">Voit yleensä tunnistaa käyttäjän oletuskoontinäytön on asetettu, jos **Aseta oletukseksi** -painike ei näy dashboard komentopalkki.</span><span class="sxs-lookup"><span data-stu-id="90235-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="90235-106">Käyttäjän oletuskoontinäytön ohittaa kaikki muut oletusarvon raporttinäkymät, vaikka nykyinen app ei ole käyttäjän oletuskoontinäytön.</span><span class="sxs-lookup"><span data-stu-id="90235-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="90235-107">Käytä seuraavaa kiertotapaa, poista niiden oletuskoontinäytöksi.</span><span class="sxs-lookup"><span data-stu-id="90235-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="90235-108">Luo uusi oma dashboard.</span><span class="sxs-lookup"><span data-stu-id="90235-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="90235-109">Määrittää, että uusi dashboard käyttäjä.</span><span class="sxs-lookup"><span data-stu-id="90235-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="90235-110">Poista tämä koontinäyttö.</span><span class="sxs-lookup"><span data-stu-id="90235-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="90235-111">Raporttinäkymät on asetettu SiteMap</span><span class="sxs-lookup"><span data-stu-id="90235-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="90235-112">Olet ehkä määrittänyt dashboard valitsemalla ja valitsemalla ”Aseta oletukseksi” mukauttaminen järjestelmässä organisaation oletuskoontinäytöksi.</span><span class="sxs-lookup"><span data-stu-id="90235-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="90235-113">Mutta määritelty sivustokartan suunnittelija dashboard ohittavat tämän koontinäytön, jos käyttäjällä on oikeus käyttää sitä.</span><span class="sxs-lookup"><span data-stu-id="90235-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="90235-114">Jos haluat nähdä raporttinäkymät, jotka olet määrittänyt oletusarvon mukaan organisaation käyttäjille, voit joko:</span><span class="sxs-lookup"><span data-stu-id="90235-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="90235-115">Määritä tämä koontinäyttö SiteMap</span><span class="sxs-lookup"><span data-stu-id="90235-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="90235-116">Käyttäjille käyttöoikeudet määritetty sivustokartan koontinäytön poistaminen</span><span class="sxs-lookup"><span data-stu-id="90235-116">Remove access to the sitemap defined dashboard for those users</span></span>
