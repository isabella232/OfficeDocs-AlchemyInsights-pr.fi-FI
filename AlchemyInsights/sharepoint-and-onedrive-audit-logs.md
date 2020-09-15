---
title: Perinteiset SharePoint-valvonta loki raportit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662205"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="ddccb-102">SharePointin ja OneDriven valvonta lokit</span><span class="sxs-lookup"><span data-stu-id="ddccb-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="ddccb-103">SharePointin perinteiset valvonta lokit</span><span class="sxs-lookup"><span data-stu-id="ddccb-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="ddccb-104">SPO-vanha valvonta on siirretty yhdistettyyn valvonta lokiin (UAL).</span><span class="sxs-lookup"><span data-stu-id="ddccb-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="ddccb-105">Kaikki SPO:N aiemmat valvonta raportit käynnistetään nyt UAL-tilassa, ja vanhat valvonta signaalit on siirretty UAL-kohteeseen.</span><span class="sxs-lookup"><span data-stu-id="ddccb-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="ddccb-106">Keskeiset muutokset:</span><span class="sxs-lookup"><span data-stu-id="ddccb-106">Key changes:</span></span>

* <span data-ttu-id="ddccb-107">Rajaus ei ole käytettävissä valmiutensa mukaan.</span><span class="sxs-lookup"><span data-stu-id="ddccb-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="ddccb-108">Tiettyjen tapahtumien valitseminen tarkastusta varten ei ole käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="ddccb-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="ddccb-109">Katso [tästä asia kirjasta](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) täydellinen luettelo tarkastetuista tapahtumista, jotka ovat käytettävissä oletusarvoisesti.</span><span class="sxs-lookup"><span data-stu-id="ddccb-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="ddccb-110">**Mukautetut raportit** -kohdan **Sijainti** -vaihto ehto ei ole käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="ddccb-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="ddccb-111">**Tiedostojen avaaminen tai lataaminen** -tapahtumat-vaihto ehto ei ole käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="ddccb-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="ddccb-112">Sivustokokoelman valvonta-asetusten määrittäminen</span><span class="sxs-lookup"><span data-stu-id="ddccb-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="ddccb-113">SharePointin ja OneDriven nykyaikaiset yhtenäiset valvonta lokit vaatimustenmukaisuudesta</span><span class="sxs-lookup"><span data-stu-id="ddccb-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="ddccb-114">Yhdistetyn valvonta kirjauksen ottaminen käyttöön/poistaminen käytöstä</span><span class="sxs-lookup"><span data-stu-id="ddccb-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="ddccb-115">SharePointin tai OneDriven sisällä ei tarvita lisä määrityksiä.</span><span class="sxs-lookup"><span data-stu-id="ddccb-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="ddccb-116">Valvonta loki haun avulla voit tarkistaa, onko tiedosto (a), kansio tai käyttäjä, käyttö oikeudet:</span><span class="sxs-lookup"><span data-stu-id="ddccb-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="ddccb-117">Tiedostojen ja sivujen toiminnot</span><span class="sxs-lookup"><span data-stu-id="ddccb-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="ddccb-118">Kansio toiminnot</span><span class="sxs-lookup"><span data-stu-id="ddccb-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="ddccb-119">Jakamis-ja yhteys pyyntö aktiviteetit</span><span class="sxs-lookup"><span data-stu-id="ddccb-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="ddccb-120">Synkronointi toiminnot</span><span class="sxs-lookup"><span data-stu-id="ddccb-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="ddccb-121">Sivuston hallinta toiminnot</span><span class="sxs-lookup"><span data-stu-id="ddccb-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="ddccb-122">Lisä tietoja näiden tapahtumien hakemisesta on kohdassa [valvonta lokista hakeminen](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="ddccb-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
