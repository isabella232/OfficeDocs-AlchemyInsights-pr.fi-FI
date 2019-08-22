---
title: Valvontalokin ottaminen käyttöön ja haku
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "286"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 37ffbe6a3c94edc3b9888b1544e9e29097d3425a
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527720"
---
# <a name="enable-and-search-the-audit-log"></a><span data-ttu-id="e187f-102">Käyttöön ja etsiä valvontaloki</span><span class="sxs-lookup"><span data-stu-id="e187f-102">Enable and search the Audit log</span></span>

<span data-ttu-id="e187f-103">Etsi Office 365: n valvontalokin, toimi [seuraavasti](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="e187f-103">To search the Office 365 audit log, follow [these steps](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="e187f-104">**Exchange**</span><span class="sxs-lookup"><span data-stu-id="e187f-104">**Exchange**</span></span>

- <span data-ttu-id="e187f-105">Exchange-järjestelmänvalvojan tehtäviä valvotaan oletusarvon mukaan.</span><span class="sxs-lookup"><span data-stu-id="e187f-105">Exchange admin activities are audited by default.</span></span>

- <span data-ttu-id="e187f-106">Olemme parhaillaan käyttöön postilaatikon valvonta oletusarvoisesti Office 365: ssä.</span><span class="sxs-lookup"><span data-stu-id="e187f-106">We are in the process of enabling mailbox auditing by default in Office 365.</span></span> <span data-ttu-id="e187f-107">Siihen asti voit valvoa tai organisaation kaikkia postilaatikoita yksittäisen postilaatikon, lue [tämä artikkeli](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing).</span><span class="sxs-lookup"><span data-stu-id="e187f-107">Until then, to enable auditing for a single mailbox or for all mailboxes in your organization, see  [this article](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing).</span></span>

- <span data-ttu-id="e187f-108">Office 365-ryhmän postilaatikot ja yleiseen kansioon Exchange Online-postilaatikot eivät tue valvontaloki.</span><span class="sxs-lookup"><span data-stu-id="e187f-108">Office 365 Group mailboxes and public folder mailboxes in Exchange Online don't support audit logging.</span></span>

<span data-ttu-id="e187f-109">**SharePoint- ja OneDrive**</span><span class="sxs-lookup"><span data-stu-id="e187f-109">**SharePoint and OneDrive**</span></span>

- <span data-ttu-id="e187f-110">On tarpeen, jotta SharePoint ja OneDrive valvonnan lisämäärityksiä.</span><span class="sxs-lookup"><span data-stu-id="e187f-110">There's no additional configuration required to enable auditing for SharePoint and OneDrive.</span></span>

- <span data-ttu-id="e187f-111">SharePoint- ja OneDrive tukevat valvonnan seuraavanlaisia aktiviteetteja:</span><span class="sxs-lookup"><span data-stu-id="e187f-111">SharePoint and OneDrive support auditing the following types of activities:</span></span>

    - <span data-ttu-id="e187f-112">Tiedoston ja kansion sivun tehtävät</span><span class="sxs-lookup"><span data-stu-id="e187f-112">File, folder, and page activities</span></span>
    - <span data-ttu-id="e187f-113">Pyynnön aktiviteettien jakaminen ja käyttö</span><span class="sxs-lookup"><span data-stu-id="e187f-113">Sharing and access request activities</span></span>
    - <span data-ttu-id="e187f-114">Sivuston hallinnan tehtävät</span><span class="sxs-lookup"><span data-stu-id="e187f-114">Site administration activities</span></span>
    - <span data-ttu-id="e187f-115">Tiedoston synkronoinnin toimintaa</span><span class="sxs-lookup"><span data-stu-id="e187f-115">File synchronization activities</span></span>

- <span data-ttu-id="e187f-116">Lisätietoja muiden Office 365-palveluiden valvottuja aktiviteetteja on [tämän artikkelin taulukko](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span><span class="sxs-lookup"><span data-stu-id="e187f-116">For information about audited activities in other Office 365 services, see  [the table in this article](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>

- <span data-ttu-id="e187f-117">Tässä luettelon hakemisesta valvontalokiin kirjataan usein kysyttyjä kysymyksiä [usein kysyttyjä kysymyksiä](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions) .</span><span class="sxs-lookup"><span data-stu-id="e187f-117">Here a list of frequently asked questions [frequently asked questions](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions) about searching the audit log.</span></span>