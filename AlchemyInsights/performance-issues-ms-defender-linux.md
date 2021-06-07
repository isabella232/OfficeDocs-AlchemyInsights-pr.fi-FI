---
title: Suorituskykyongelmat Microsoft Defender for Endpointissa Linuxissa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793758"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="0c193-102">Suorituskykyongelmat Microsoft Defender for Endpointissa Linuxissa</span><span class="sxs-lookup"><span data-stu-id="0c193-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="0c193-103">Tässä artikkelissa on ohjeet Microsoft Defender for Endpointin suorituskykyongelman tunnistamiseen Linuxissa.</span><span class="sxs-lookup"><span data-stu-id="0c193-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="0c193-104">On tärkeää ensin varmistaa, että ongelma on ratkaistu uusimmalla [versiolla](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span><span class="sxs-lookup"><span data-stu-id="0c193-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="0c193-105">Aloita tutkimus tutustumaan ohjeisiin, joissa [käsitellään Microsoft Defender for Endpointin suorituskykyongelmien vianmääritys Linuxissa.](/microsoft-365/security/defender-endpoint/linux-support-perf)</span><span class="sxs-lookup"><span data-stu-id="0c193-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="0c193-106">Poikkeukset</span><span class="sxs-lookup"><span data-stu-id="0c193-106">Exclusions</span></span>

<span data-ttu-id="0c193-107">Poikkeukset voivat auttaa lieventämään suorituskykyongelmia.</span><span class="sxs-lookup"><span data-stu-id="0c193-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="0c193-108">Tarkista poikkeukset ennen aloittamista, jotta mahdolliset lisäriskit ovat tiedossa ja dokumentoitu.</span><span class="sxs-lookup"><span data-stu-id="0c193-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="0c193-109">Lisätietoja on kohdassa [Microsoft Defender for Endpointin](/microsoft-365/security/defender-endpoint/linux-exclusions)poikkeusten määrittäminen ja vahvistaminen Linuxissa.</span><span class="sxs-lookup"><span data-stu-id="0c193-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="0c193-110">Jos sinulla on useita tiedostoja & pois jätettäväksi ja ne kaikki ovat samassa päätepisteessä, voi olla helpompaa jättää päätepiste pois.</span><span class="sxs-lookup"><span data-stu-id="0c193-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="0c193-111">Helmikuun julkaisusta 101.22.80 alkaen voit jättää pois kokonaisen päätepisteen.</span><span class="sxs-lookup"><span data-stu-id="0c193-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="0c193-112">Jos esimerkiksi /mnt/backup on mountpoint, voit lisätä /mnt/backup poissulkevien luetteloon suorittamalla tämän komennon:</span><span class="sxs-lookup"><span data-stu-id="0c193-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="0c193-113">**Huomautus:** Ohittamisen lisääminen lisää riskiä, että haittaohjelmia ei havaita ja että se on käsiteltävä ja otettava käyttöön huolellisesti.</span><span class="sxs-lookup"><span data-stu-id="0c193-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="0c193-114">Tarvitsetko apua?</span><span class="sxs-lookup"><span data-stu-id="0c193-114">Need Help?</span></span>

<span data-ttu-id="0c193-115">Voit auttaa sinua tehokkaimmalla tavalla keräämalla diagnostiikkatiedot ennen tukitapauksen avaamista.</span><span class="sxs-lookup"><span data-stu-id="0c193-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
