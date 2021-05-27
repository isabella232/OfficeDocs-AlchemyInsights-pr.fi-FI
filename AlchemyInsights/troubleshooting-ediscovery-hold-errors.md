---
title: Ediscovery-sovelluksen vianmääritys sisältää virheitä
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676148"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="287d4-102">Ediscovery-sovelluksen vianmääritys sisältää virheitä</span><span class="sxs-lookup"><span data-stu-id="287d4-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="287d4-103">Onko eDiscovery-pitoon liittyviä ongelmia?</span><span class="sxs-lookup"><span data-stu-id="287d4-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="287d4-104">Seuraavassa on joitakin parhaita käytäntöjä, jotka kannattaa ottaa huomioon:</span><span class="sxs-lookup"><span data-stu-id="287d4-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="287d4-105">Tarkista pitojakauman tila.</span><span class="sxs-lookup"><span data-stu-id="287d4-105">Check the hold distribution status.</span></span>  <span data-ttu-id="287d4-106">Jos tila **on Käytössä (Odottaa) tai** Ei käytössä **(Odottaa),** odota, että pitojakelu on valmis.</span><span class="sxs-lookup"><span data-stu-id="287d4-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="287d4-107">Yhdistä eDiscovery-pitopäivitykset yhdeksi joukkopyynnöksi sen sijaan, että päivität käytännön toistuvasti kullekin tapahtumalle.</span><span class="sxs-lookup"><span data-stu-id="287d4-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="287d4-108">Suorita Set-CaseHoldPolicy <policyname> -Yritä uudelleenjakamista Tietoturva- ja yhteensopivuuskeskuksen Powershellissä.</span><span class="sxs-lookup"><span data-stu-id="287d4-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="287d4-109">Lisätietoja on Näyttöyhteys [powershellin tietoturva& hallintakeskuksessa.](/powershell/exchange/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="287d4-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="287d4-110">Ohjeet näiden asetusten tarkistamiseen sekä eDiscovery-pitoongelmien lieventämiseen ja ratkaisemiseen liittyvät parhaat käytännöt ovat kohdassa [eDiscovery-pitovirheiden vianmääritys.](/microsoft-365/compliance/hold-distribution-errors)</span><span class="sxs-lookup"><span data-stu-id="287d4-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="287d4-111">Lisätietoja muiden yleisimmät eDiscovery-ongelmien vianmäärityksestä ovat kohdassa [eDiscovery-ongelmien tutkiminen, vianmääritys ja ratkaiseminen.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)</span><span class="sxs-lookup"><span data-stu-id="287d4-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
