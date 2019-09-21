---
title: Perinteisen SharePointin valvonta lokin raportit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068020"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="cd24e-102">SharePointin ja OneDriven valvonta lokit</span><span class="sxs-lookup"><span data-stu-id="cd24e-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="cd24e-103">**SharePointin ja OneDriven modernit yhtenäiset valvonta lokit vaatimustenmukaisuudesta**</span><span class="sxs-lookup"><span data-stu-id="cd24e-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="cd24e-104">Yhtenäisen valvonta lokin ottaminen käyttöön ja poistaminen käytöstä</span><span class="sxs-lookup"><span data-stu-id="cd24e-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="cd24e-105">SharePointin tai OneDriven sisällä ei tarvita lisä määrityksiä.</span><span class="sxs-lookup"><span data-stu-id="cd24e-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="cd24e-106">Käytä valvonnan kirjaamis hakua tiedostojen, kansioiden, käyttäjien ja käyttö oikeuksien tarkistustyö:</span><span class="sxs-lookup"><span data-stu-id="cd24e-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="cd24e-107">Tiedostojen ja sivujen toiminnot</span><span class="sxs-lookup"><span data-stu-id="cd24e-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="cd24e-108">Kansion aktiviteetit</span><span class="sxs-lookup"><span data-stu-id="cd24e-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="cd24e-109">Jakamis-ja käyttö oikeus pyyntöjen toiminnot</span><span class="sxs-lookup"><span data-stu-id="cd24e-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="cd24e-110">Synkronointi toiminnot</span><span class="sxs-lookup"><span data-stu-id="cd24e-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="cd24e-111">Sivuston hallinta toiminnot</span><span class="sxs-lookup"><span data-stu-id="cd24e-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="cd24e-112">Lisä tietoja näiden tapahtumien hakemista on kohdassa [valvonta lokin](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)hakeminen.</span><span class="sxs-lookup"><span data-stu-id="cd24e-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="cd24e-113">**SharePoint Classicin valvonta lokit**</span><span class="sxs-lookup"><span data-stu-id="cd24e-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="cd24e-114">Siirsimme SPO Legacy Audit-valvonnan yhtenäiseen valvonta lokiin (UAL).</span><span class="sxs-lookup"><span data-stu-id="cd24e-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="cd24e-115">Tämä tarkoittaa lähinnä sitä, että kaikki SPO Legacy-auditointi raportit ovat nyt powered by UAL, ja vanhoja valvonta signaaleja on siirretty UAL.</span><span class="sxs-lookup"><span data-stu-id="cd24e-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="cd24e-116">Keskeiset muutokset:</span><span class="sxs-lookup"><span data-stu-id="cd24e-116">Key changes:</span></span>

- <span data-ttu-id="cd24e-117">Ominaisuuksien rajaaminen ei ole mahdollista.</span><span class="sxs-lookup"><span data-stu-id="cd24e-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="cd24e-118">Osa, jossa valitset tiettyjä valvonta tapahtumia, ei ole käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="cd24e-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="cd24e-119">Katso [tästä asia kirjasta](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) täydellinen luettelo tarkastetuista tapahtumista, jotka ovat oletusarvoisesti käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="cd24e-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="cd24e-120">**Mukautetut raportit** -kohdan sijainti-vaihto ehto ei ole käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="cd24e-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="cd24e-121">"Asia kirjojen avaaminen tai lataaminen"-tapahtumat eivät ole käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="cd24e-121">“Opening or downloading documents” events is NOT available.</span></span> 

