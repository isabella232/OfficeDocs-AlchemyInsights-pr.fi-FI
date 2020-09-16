---
title: Vanhojen eDiscoveryn poistaminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727780"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="329ff-102">Vanhojen eDiscoveryn poistaminen</span><span class="sxs-lookup"><span data-stu-id="329ff-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="329ff-103">Microsoft 365-yhteensopivuus keskuksen uusien ja parannettujen eDiscoveryn toimintojen tuloksena seuraavat vanhat eDiscoveryn työkalut ja komentosovelmat poistuvat käytöstä lähikuukausina:</span><span class="sxs-lookup"><span data-stu-id="329ff-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="329ff-104">Exchange-hallinta keskuksen käytössä oleva [etsimis](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) -ja pito [paikka](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) .</span><span class="sxs-lookup"><span data-stu-id="329ff-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="329ff-105">Exchange Online PowerShellin cmdlet-komentosovelmat, jotka tukevat sijaintia etsimis-ja paikallaan.</span><span class="sxs-lookup"><span data-stu-id="329ff-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="329ff-106">(Nämä cmdlet-komentosovelmat tunnistetaan yhteisesti \*-posti laatikon haun cmdlet-komentosovelmat.) Tämä sisältää seuraavat cmdlet-komento:</span><span class="sxs-lookup"><span data-stu-id="329ff-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="329ff-107">Uusi-Mailposti-haku</span><span class="sxs-lookup"><span data-stu-id="329ff-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="329ff-108">Käynnistä-posti laatikon haku</span><span class="sxs-lookup"><span data-stu-id="329ff-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="329ff-109">Pysäytä-posti laatikon haku</span><span class="sxs-lookup"><span data-stu-id="329ff-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="329ff-110">Asetukset-posti laatikon haku</span><span class="sxs-lookup"><span data-stu-id="329ff-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="329ff-111">[Search-Mailbox-cmdlet-](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) vaihto Exchange Online PowerShellissä.</span><span class="sxs-lookup"><span data-stu-id="329ff-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="329ff-112">Seuraavat Exchange Web Services-ohjelmointi raja pinnan toiminnot:</span><span class="sxs-lookup"><span data-stu-id="329ff-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="329ff-113">Getsearchtablemailboxes</span><span class="sxs-lookup"><span data-stu-id="329ff-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="329ff-114">Asetholdonposti laatikot</span><span class="sxs-lookup"><span data-stu-id="329ff-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="329ff-115">Geosholdonpostilaatikkoposti laatikot</span><span class="sxs-lookup"><span data-stu-id="329ff-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="329ff-116">Advanced eDiscoveryn v 1.0</span><span class="sxs-lookup"><span data-stu-id="329ff-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="329ff-117">**Eläkkeelle siirtymisen aika Jana**:</span><span class="sxs-lookup"><span data-stu-id="329ff-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="329ff-118">**1. heinä kuuta 2020** Et voi enää luoda uusia hakuja ja pitää niitä, mutta voit suorittaa, muokata ja poistaa olemassa olevia hakuja omalla vastuullasi.</span><span class="sxs-lookup"><span data-stu-id="329ff-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="329ff-119">Microsoft-tuki ei enää tue paikan päällä olevaa eDiscoverya & pätee EAC:ssä.</span><span class="sxs-lookup"><span data-stu-id="329ff-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="329ff-120">**1. loka kuuta, 2020** Paikan päällä oleva eDiscoveryn &-toiminto on käytettävissä vain luku-tilassa, joten voit poistaa vain olemassa olevat haut ja ruumat.</span><span class="sxs-lookup"><span data-stu-id="329ff-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="329ff-121">Lisä **tietoja on kohdassa**:</span><span class="sxs-lookup"><span data-stu-id="329ff-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="329ff-122">Vanhojen eDiscoveryn hakujen ja Pitojen siirtäminen Microsoft 365-yhteensopivuus keskukseen</span><span class="sxs-lookup"><span data-stu-id="329ff-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="329ff-123">Vanhojen eDiscoveryn poistaminen</span><span class="sxs-lookup"><span data-stu-id="329ff-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="329ff-124">Usein kysyttyjä kysymyksiä paikasta ja paikasta</span><span class="sxs-lookup"><span data-stu-id="329ff-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



