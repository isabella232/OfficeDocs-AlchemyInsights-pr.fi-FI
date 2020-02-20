---
title: Vanhojen eDiscovery-työkalujen eläkkeelle siirtyminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157572"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="2aa3f-102">Vanhojen eDiscovery-työkalujen eläkkeelle siirtyminen</span><span class="sxs-lookup"><span data-stu-id="2aa3f-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="2aa3f-103">Microsoft 365 Compliance Centerin uusien ja parannettujen eDiscovery-toimintojen seurauksena seuraavat vanhat eDiscovery-työkalut ja -komennot poistetaan käytöstä tulevina kuukausina:</span><span class="sxs-lookup"><span data-stu-id="2aa3f-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="2aa3f-104">[Exchange-hallintakeskuksessa on käytössä eDiscovery-](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) ja [In-Place-pitoja.](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)</span><span class="sxs-lookup"><span data-stu-id="2aa3f-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="2aa3f-105">Exchange Online PowerShell -cmdlet-komennot, jotka tukevat in-place eDiscovery- ja In-Place-pitoja.</span><span class="sxs-lookup"><span data-stu-id="2aa3f-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="2aa3f-106">(Nämä cmdlet-komennot tunnistetaan yhteisesti \*-MailboxSearch-cmdlet-komennoiksi.) Tämä sisältää seuraavat cmdlet-komennot:</span><span class="sxs-lookup"><span data-stu-id="2aa3f-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="2aa3f-107">Uusi postilaatikkohaku</span><span class="sxs-lookup"><span data-stu-id="2aa3f-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="2aa3f-108">Käynnistä postilaatikkohaku</span><span class="sxs-lookup"><span data-stu-id="2aa3f-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="2aa3f-109">Stop-MailboxSearch -haku</span><span class="sxs-lookup"><span data-stu-id="2aa3f-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="2aa3f-110">Aseta postilaatikkohaku</span><span class="sxs-lookup"><span data-stu-id="2aa3f-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="2aa3f-111">Exchange Online PowerShellin [hakupostilaatikon](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet-komento.</span><span class="sxs-lookup"><span data-stu-id="2aa3f-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="2aa3f-112">Seuraavat Exchange Web Services -ohjelmointirajapinnan toiminnot:</span><span class="sxs-lookup"><span data-stu-id="2aa3f-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="2aa3f-113">GetSearchableMailboxes -postilaatikot</span><span class="sxs-lookup"><span data-stu-id="2aa3f-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="2aa3f-114">Aseta HoldOnPostilaatikot</span><span class="sxs-lookup"><span data-stu-id="2aa3f-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="2aa3f-115">GetHoldOnPostilaatikot</span><span class="sxs-lookup"><span data-stu-id="2aa3f-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="2aa3f-116">Office 365 Advanced eDiscovery v1.0 (Office 365 Advanced eDiscovery v1.0) Office 365 Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="2aa3f-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="2aa3f-117">**Eläkkeelle siirtymisen aikataulu:**</span><span class="sxs-lookup"><span data-stu-id="2aa3f-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="2aa3f-118">1.4.2020: Et voi luoda uusia hakuja ja pitoja, mutta voit silti suorittaa, muokata ja poistaa olemassa olevia hakuja omalla vastuullasi.</span><span class="sxs-lookup"><span data-stu-id="2aa3f-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="2aa3f-119">Microsoftin tuki ei enää tue EAC:n in Place eDiscovery & -pitoja.</span><span class="sxs-lookup"><span data-stu-id="2aa3f-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="2aa3f-120">1.7.2020: EAC:n in Place eDiscovery & Holds -toiminto sijoitetaan vain luku -tilaan.</span><span class="sxs-lookup"><span data-stu-id="2aa3f-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="2aa3f-121">Tämä tarkoittaa, että voit poistaa vain olemassa olevat haut ja pidot.</span><span class="sxs-lookup"><span data-stu-id="2aa3f-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="2aa3f-122">**Lisätietoja on kohdassa**:</span><span class="sxs-lookup"><span data-stu-id="2aa3f-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="2aa3f-123">Vanhojen eDiscovery-hakujen ja -pitojen siirtäminen Microsoft 365 -yhteensopivuuskeskukseen</span><span class="sxs-lookup"><span data-stu-id="2aa3f-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="2aa3f-124">Vanhojen eDiscovery-työkalujen eläkkeelle siirtyminen</span><span class="sxs-lookup"><span data-stu-id="2aa3f-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="2aa3f-125">Usein kysyttyjä kysymyksiä in-place eDiscovery- ja In-Place-ruuista</span><span class="sxs-lookup"><span data-stu-id="2aa3f-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



