---
title: Project Online on vain luku-tilassa
ms.author: pebaum
author: pebaum
manager: pamg
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1776"
- "9000205"
ms.openlocfilehash: ad2a9f95bf30708772edb166945f3f42e0f1f503
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801649"
---
# <a name="project-online-is-in-a-read-only-state"></a><span data-ttu-id="fde32-102">Project Online on vain luku-tilassa</span><span class="sxs-lookup"><span data-stu-id="fde32-102">Project Online is in a read-only state</span></span>

<span data-ttu-id="fde32-103">Project Online voi saavuttaa vain luku-tilassa kolme yleistä syytä:</span><span class="sxs-lookup"><span data-stu-id="fde32-103">There are three common reasons why Project Online may reach a read-only state:</span></span>

1. <span data-ttu-id="fde32-104">Organisaatioilla on vain Project Online Essentials-käyttö oikeus (a).</span><span class="sxs-lookup"><span data-stu-id="fde32-104">Organizations have a Project Online Essentials license(s) only.</span></span> <span data-ttu-id="fde32-105">Tämä ei riitä sivuston pitämiseksi hengissä, ja se saa lopulta valmiiksi valmistelun.</span><span class="sxs-lookup"><span data-stu-id="fde32-105">This isn't enough to keep the site alive and it will eventually get de-provisioned.</span></span><span data-ttu-id="fde32-106">Sivusto sijoitetaan vain luku-tilaan, jotta järjestelmänvalvojat tietävät, että jokin on vialla ja että hän voi hankkia oikeat käyttö oikeudet.</span><span class="sxs-lookup"><span data-stu-id="fde32-106"> We place the site in a read-only state so that Admins know something is wrong and can acquire the correct licenses.</span></span> <span data-ttu-id="fde32-107">Järjestelmänvalvojien on lisättävä Project Online Professional-ja/tai Premium-käyttö oikeus.</span><span class="sxs-lookup"><span data-stu-id="fde32-107">Admins will need to add a Project Online Professional and/or Premium license.</span></span> <span data-ttu-id="fde32-108">Sivusto tulee ulos vain luku-tilassa.</span><span class="sxs-lookup"><span data-stu-id="fde32-108">The site will come out of read-only at that point.</span></span> <span data-ttu-id="fde32-109">Lisä tietoja on Ohje aiheessa [projektin hallinta ratkaisujen vertaileminen](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span><span class="sxs-lookup"><span data-stu-id="fde32-109">For more info, see [Compare Project Management Solutions](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span></span>
2. <span data-ttu-id="fde32-110">Määritetty kiintiö on saavutettu.</span><span class="sxs-lookup"><span data-stu-id="fde32-110">Assigned quota has been reached.</span></span> <span data-ttu-id="fde32-111">Lisä tietoja on kohdassa [Project Web App-kiintiö](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span><span class="sxs-lookup"><span data-stu-id="fde32-111">For more info, see [Project Web App Quota](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span></span> <span data-ttu-id="fde32-112">Tarkista [Project Onlinen aikajaksotettujen raportti tietojen koonti asetusten määrittäminen](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) , jotta näet, miten raportin rakeisuus saattaa vaikuttaa kiintiön käyttöön.</span><span class="sxs-lookup"><span data-stu-id="fde32-112">Check [Configure rollup of timephased reporting data in Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) to see how reporting granularity may impact quota usage.</span></span>
3. <span data-ttu-id="fde32-113">Vain luku-tila voi olla hyvin väliaikainen ehto, joka voi ilmetä huollon aikana.</span><span class="sxs-lookup"><span data-stu-id="fde32-113">Read-only can be a very temporary condition that can occur during maintenance.</span></span> <span data-ttu-id="fde32-114">Useimmat huolto toimet eivät ole edes havaittavissa asiakkaillemme, mutta niitä ei useinkaan näy, mutta vain luku-tilassa on aikaa.</span><span class="sxs-lookup"><span data-stu-id="fde32-114">Most maintenance is not even noticed by our customers and you will not often see this, but there are times when short periods of read-only are experienced.</span></span>
