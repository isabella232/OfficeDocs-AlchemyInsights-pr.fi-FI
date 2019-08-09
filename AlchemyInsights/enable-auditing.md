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
ms.openlocfilehash: 8c965cb1c2b6a4cb46b5c1b0145932c4c54ba97d
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270525"
---
# <a name="enable-and-search-audit-log"></a><span data-ttu-id="699b5-102">Valvontalokin ottaminen käyttöön ja haku</span><span class="sxs-lookup"><span data-stu-id="699b5-102">Enable and search Audit log</span></span>

<span data-ttu-id="699b5-103">Etsi Office 365: n valvontalokin, toimi [seuraavasti](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="699b5-103">To search the Office 365 audit log, follow [these steps](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="699b5-104">**Exchange**</span><span class="sxs-lookup"><span data-stu-id="699b5-104">**Exchange**</span></span>

- <span data-ttu-id="699b5-105">Exchange-järjestelmänvalvojan tehtäviä valvotaan oletusarvon mukaan.</span><span class="sxs-lookup"><span data-stu-id="699b5-105">Exchange admin activities are audited by default.</span></span>

- <span data-ttu-id="699b5-106">Olemme parhaillaan käyttöön postilaatikon valvonta oletusarvoisesti Office 365: ssä.</span><span class="sxs-lookup"><span data-stu-id="699b5-106">We are in the process of enabling mailbox auditing by default in Office 365.</span></span> <span data-ttu-id="699b5-107">Siihen asti voit valvoa tai organisaation kaikkia postilaatikoita yksittäisen postilaatikon, lue [tämä artikkeli](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing).</span><span class="sxs-lookup"><span data-stu-id="699b5-107">Until then, to enable auditing for a single mailbox or for all mailboxes in your organization, see  [this article](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing).</span></span>

- <span data-ttu-id="699b5-108">Office 365-ryhmän postilaatikot ja yleiseen kansioon Exchange Online-postilaatikot eivät tue valvontaloki.</span><span class="sxs-lookup"><span data-stu-id="699b5-108">Office 365 Group mailboxes and public folder mailboxes in Exchange Online don't support audit logging.</span></span>

<span data-ttu-id="699b5-109">**SharePoint- ja OneDrive**</span><span class="sxs-lookup"><span data-stu-id="699b5-109">**SharePoint and OneDrive**</span></span>

- <span data-ttu-id="699b5-110">On tarpeen, jotta SharePoint ja OneDrive valvonnan lisämäärityksiä.</span><span class="sxs-lookup"><span data-stu-id="699b5-110">There's no additional configuration required to enable auditing for SharePoint and OneDrive.</span></span>

- <span data-ttu-id="699b5-111">SharePoint- ja OneDrive tukevat valvonnan seuraavanlaisia aktiviteetteja:</span><span class="sxs-lookup"><span data-stu-id="699b5-111">SharePoint and OneDrive support auditing the following types of activities:</span></span>

    - <span data-ttu-id="699b5-112">Tiedoston ja kansion sivun tehtävät</span><span class="sxs-lookup"><span data-stu-id="699b5-112">File, folder, and page activities</span></span>
    - <span data-ttu-id="699b5-113">Pyynnön aktiviteettien jakaminen ja käyttö</span><span class="sxs-lookup"><span data-stu-id="699b5-113">Sharing and access request activities</span></span>
    - <span data-ttu-id="699b5-114">Sivuston hallinnan tehtävät</span><span class="sxs-lookup"><span data-stu-id="699b5-114">Site administration activities</span></span>
    - <span data-ttu-id="699b5-115">Tiedoston synkronoinnin toimintaa</span><span class="sxs-lookup"><span data-stu-id="699b5-115">File synchronization activities</span></span>

- <span data-ttu-id="699b5-116">Lisätietoja muiden Office 365-palveluiden valvottuja aktiviteetteja on [tämän artikkelin taulukko](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span><span class="sxs-lookup"><span data-stu-id="699b5-116">For information about audited activities in other Office 365 services, see  [the table in this article](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>

- <span data-ttu-id="699b5-117">Tässä luettelon hakemisesta valvontalokiin kirjataan usein kysyttyjä kysymyksiä [usein kysyttyjä kysymyksiä](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions) .</span><span class="sxs-lookup"><span data-stu-id="699b5-117">Here a list of frequently asked questions [frequently asked questions](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions) about searching the audit log.</span></span>