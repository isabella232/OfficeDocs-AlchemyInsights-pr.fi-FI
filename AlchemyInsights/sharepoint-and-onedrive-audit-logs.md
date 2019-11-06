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
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992615"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="8f596-102">SharePointin ja OneDriven valvonta lokit</span><span class="sxs-lookup"><span data-stu-id="8f596-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="8f596-103">SharePoint Classicin valvonta lokit</span><span class="sxs-lookup"><span data-stu-id="8f596-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="8f596-104">SPO Legacy-valvonta siirrettiin yhtenäiseen valvonta lokiin (UAL).</span><span class="sxs-lookup"><span data-stu-id="8f596-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="8f596-105">Kaikki SPO Legacy-auditointi raportit toimivat nyt UAL-järjestelmän kautta, ja aiemmat auditointi signaalit on siirretty UAL-järjestelmään.</span><span class="sxs-lookup"><span data-stu-id="8f596-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="8f596-106">Keskeiset muutokset:</span><span class="sxs-lookup"><span data-stu-id="8f596-106">Key changes:</span></span>

* <span data-ttu-id="8f596-107">Trimmaus ei ole käytettävissä ominaisuus.</span><span class="sxs-lookup"><span data-stu-id="8f596-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="8f596-108">Tiettyjen tapahtumien valitseminen valvomatta ei ole käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="8f596-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="8f596-109">Katso [tästä asia kirjasta](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) täydellinen luettelo tarkastetuista tapahtumista, jotka ovat oletusarvoisesti käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="8f596-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="8f596-110">**Mukautettujen raporttien** **Sijainti** vaihtoehto ei ole käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="8f596-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="8f596-111">**Avaus-tai lataus asiakirjojen** tapahtumat-vaihto ehto ei ole käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="8f596-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="8f596-112">Sivustokokoelman valvonta-asetusten määrittäminen</span><span class="sxs-lookup"><span data-stu-id="8f596-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="8f596-113">SharePointin ja OneDriven modernit yhtenäiset valvonta lokit vaatimustenmukaisuudesta</span><span class="sxs-lookup"><span data-stu-id="8f596-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="8f596-114">Yhtenäisen valvonta lokin ottaminen käyttöön ja poistaminen käytöstä</span><span class="sxs-lookup"><span data-stu-id="8f596-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="8f596-115">SharePointin tai OneDriven sisällä ei tarvita lisä määrityksiä.</span><span class="sxs-lookup"><span data-stu-id="8f596-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="8f596-116">Käytä valvonnan kirjaamis hakua tiedostojen, kansioiden, käyttäjien ja käyttö oikeuksien tarkistustyö:</span><span class="sxs-lookup"><span data-stu-id="8f596-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="8f596-117">Tiedostojen ja sivujen toiminnot</span><span class="sxs-lookup"><span data-stu-id="8f596-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="8f596-118">Kansion aktiviteetit</span><span class="sxs-lookup"><span data-stu-id="8f596-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="8f596-119">Jakamis-ja käyttö oikeus pyyntöjen toiminnot</span><span class="sxs-lookup"><span data-stu-id="8f596-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="8f596-120">Synkronointi toiminnot</span><span class="sxs-lookup"><span data-stu-id="8f596-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="8f596-121">Sivuston hallinta toiminnot</span><span class="sxs-lookup"><span data-stu-id="8f596-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="8f596-122">Lisä tietoja näiden tapahtumien hakemista on kohdassa [valvonta lokin](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)hakeminen.</span><span class="sxs-lookup"><span data-stu-id="8f596-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
