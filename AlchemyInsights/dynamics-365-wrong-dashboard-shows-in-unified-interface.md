---
title: Dynamics 365-Dynamics 365 Unified Interface-liittymän väärät koonti näyttöjen esitykset
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528548"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="024d3-102">Dynamics 365 Unified Interface-liittymän väärät koonti näyttöjen esitykset</span><span class="sxs-lookup"><span data-stu-id="024d3-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="024d3-103">On useita syitä, miksi saatat nähdä eri koonti näytön kuin mitä odotat:</span><span class="sxs-lookup"><span data-stu-id="024d3-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="024d3-104">Käyttäjä on määrittänyt käyttäjän oletus koonti näytön</span><span class="sxs-lookup"><span data-stu-id="024d3-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="024d3-105">Yleensä voit tunnistaa käyttäjän oletus koonti näytön, jos **Aseta oletus** arvoksi-painike ei näy koonti näytön komento palkissa.</span><span class="sxs-lookup"><span data-stu-id="024d3-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="024d3-106">Käyttäjän oletus koonti näyttö ohittaa kaikki muut oletus koonti näytöt, vaikka käyttäjän oletus koonti näyttö ei olisi nykyisessä sovelluksessa.</span><span class="sxs-lookup"><span data-stu-id="024d3-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="024d3-107">Poista oletus koonti näytön asetus käytöstä seuraavan kierto tavan avulla.</span><span class="sxs-lookup"><span data-stu-id="024d3-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="024d3-108">Luo uusi henkilökohtainen koonti näyttö.</span><span class="sxs-lookup"><span data-stu-id="024d3-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="024d3-109">Määritä uusi koonti näyttö käyttäjän oletus arvoksi.</span><span class="sxs-lookup"><span data-stu-id="024d3-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="024d3-110">Poista kyseinen koonti näyttö.</span><span class="sxs-lookup"><span data-stu-id="024d3-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="024d3-111">Koonti näyttö on määritetty sivustokartassa</span><span class="sxs-lookup"><span data-stu-id="024d3-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="024d3-112">Olet ehkä määrittänyt organisaation oletus koonti näytön valitsemalla koonti näytön ja valitsemalla "Määritä oletukseksi" kohdassa "Mukauta järjestelmää".</span><span class="sxs-lookup"><span data-stu-id="024d3-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="024d3-113">Sivustokartan suunnittelu ohjelmassa määritetty koonti näyttö ohittaa kuitenkin tämän koonti näytön, jos käyttäjällä on siihen käyttö oikeus.</span><span class="sxs-lookup"><span data-stu-id="024d3-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="024d3-114">Jotta käyttäjät näkevät koonti näytön, jonka olet määrittänyt organisaation oletus arvoksi, voit joko:</span><span class="sxs-lookup"><span data-stu-id="024d3-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="024d3-115">Määritä tämä koonti näyttö sivustokartassa</span><span class="sxs-lookup"><span data-stu-id="024d3-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="024d3-116">Poista käyttö oikeudet sivustokartan määritettyyn koonti näyttöön näille käyttäjille</span><span class="sxs-lookup"><span data-stu-id="024d3-116">Remove access to the sitemap defined dashboard for those users</span></span>
