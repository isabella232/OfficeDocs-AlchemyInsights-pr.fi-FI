---
title: Vanhojen eDiscovery-työkalujen käytöstä poisto
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798546"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="ba3d3-102">Vanhojen eDiscovery-työkalujen käytöstä poisto</span><span class="sxs-lookup"><span data-stu-id="ba3d3-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="ba3d3-103">Microsoft 365 -yhteensopivuuskeskuksen uusien ja parannettujen eDiscovery-toimintojen ansiosta seuraavat vanhat eDiscovery-työkalut ja -komentojen komennot eivät enää ole käytettävissä seuraavien kuukausien aikana:</span><span class="sxs-lookup"><span data-stu-id="ba3d3-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="ba3d3-104">[Aseta eDiscovery-pito](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [ja pitopalvelu](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) käyttöön Exchange-hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="ba3d3-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="ba3d3-105">Exchange Onlinen PowerShell-cmdlet-komennot, jotka In-Place eDiscovery- In-Place pitopalveluissa.</span><span class="sxs-lookup"><span data-stu-id="ba3d3-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="ba3d3-106">(Nämä cmdlet-komennot tunnistetaan yhteisesti \*-MailboxSearch-cmdlet-komennoiksi.) Tämä sisältää seuraavat cmdlet-komennot:</span><span class="sxs-lookup"><span data-stu-id="ba3d3-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="ba3d3-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ba3d3-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="ba3d3-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ba3d3-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="ba3d3-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ba3d3-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="ba3d3-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ba3d3-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="ba3d3-111">Exchange Online [PowerShellin Search-Mailbox-cmdlet-komento.](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="ba3d3-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="ba3d3-112">Seuraavat toiminnot Exchange-verkkopalveluiden ohjelmointirajapinnassa:</span><span class="sxs-lookup"><span data-stu-id="ba3d3-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="ba3d3-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="ba3d3-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="ba3d3-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ba3d3-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="ba3d3-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ba3d3-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="ba3d3-116">Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="ba3d3-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="ba3d3-117">**Aikajana käytöstä poistolle:**</span><span class="sxs-lookup"><span data-stu-id="ba3d3-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="ba3d3-118">**1. heinäkuuta 2020** Et voi enää luoda uusia hakuja ja pitoja, mutta voit suorittaa, muokata ja poistaa aiemmin luotuja hakuja omalla vastuullasi.</span><span class="sxs-lookup"><span data-stu-id="ba3d3-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="ba3d3-119">Microsoft-tuki ei enää In-Place eDiscovery& pitoa EAC:ssä.</span><span class="sxs-lookup"><span data-stu-id="ba3d3-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="ba3d3-120">**1. lokakuuta 2020** In-Place eDiscovery & EAC:n Pitotoiminnot sijoitetaan vain luku -tilaan, joten voit poistaa vain aiemmin luodut haut ja pitotoiminnot.</span><span class="sxs-lookup"><span data-stu-id="ba3d3-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="ba3d3-121">**Lisätietoja on kohdassa:**</span><span class="sxs-lookup"><span data-stu-id="ba3d3-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="ba3d3-122">Vanhojen eDiscovery-hakujen ja -pitojen siirtäminen Microsoft 365 -yhteensopivuuskeskukseen</span><span class="sxs-lookup"><span data-stu-id="ba3d3-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="ba3d3-123">Vanhojen eDiscovery-työkalujen käytöstä poisto</span><span class="sxs-lookup"><span data-stu-id="ba3d3-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="ba3d3-124">Usein kysyttyjä kysymyksiä eDiscoveryIn-Place ja In-Place pitoon liittyen</span><span class="sxs-lookup"><span data-stu-id="ba3d3-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



