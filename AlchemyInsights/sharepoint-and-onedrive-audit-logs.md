---
title: Perinteiset SharePoint-valvontalokiraportit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509597"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="72503-102">SharePoint- ja OneDrive-valvontalokit</span><span class="sxs-lookup"><span data-stu-id="72503-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="72503-103">SharePointin perinteiset valvontalokit</span><span class="sxs-lookup"><span data-stu-id="72503-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="72503-104">SPO:n vanha valvonta siirrettiin yhtenäiseen valvontalokiin (UAL).</span><span class="sxs-lookup"><span data-stu-id="72503-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="72503-105">Kaikki SPO:n vanhat auditointiraportit saavat nyt virtaa UAL:n kautta, ja vanhat valvontasignaalit on siirretty UAL-ilmoitukseen.</span><span class="sxs-lookup"><span data-stu-id="72503-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="72503-106">Keskeiset muutokset:</span><span class="sxs-lookup"><span data-stu-id="72503-106">Key changes:</span></span>

* <span data-ttu-id="72503-107">Trimmaus ei ole käytettävissä lisävarusteena.</span><span class="sxs-lookup"><span data-stu-id="72503-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="72503-108">Tiettyjen tarkettavissa olevien tapahtumien valitseminen ei ole käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="72503-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="72503-109">Tässä [asiakirjassa](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) on täydellinen luettelo oletusarvoisesti käytettävissä olevista valvotuista tapahtumista.</span><span class="sxs-lookup"><span data-stu-id="72503-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="72503-110">**Mukautetut raportit -kohdan** **Sijainti-vaihtoehto** ei ole käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="72503-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="72503-111">**Asiakirjojen avaaminen tai lataaminen** -vaihtoehto ei ole käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="72503-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="72503-112">Sivustokokoelman valvonta-asetusten määrittäminen</span><span class="sxs-lookup"><span data-stu-id="72503-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="72503-113">SharePoint- ja OneDrive Modern Unified Audit -lokit vaatimustenmukaisuudesta</span><span class="sxs-lookup"><span data-stu-id="72503-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="72503-114">Yhtenäisen valvonnan kirjaamisen ottaminen käyttöön tai poistaminen käytöstä</span><span class="sxs-lookup"><span data-stu-id="72503-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="72503-115">Lisämäärityksiä ei tarvita SharePointissa tai OneDrivessa.</span><span class="sxs-lookup"><span data-stu-id="72503-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="72503-116">Valvontalokihaun avulla voit tarkistaa tiedostojen, kansioiden, käyttäjien ja käyttöoikeuksien aktiviteetit:</span><span class="sxs-lookup"><span data-stu-id="72503-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="72503-117">Tiedosto- ja sivutoiminnot</span><span class="sxs-lookup"><span data-stu-id="72503-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="72503-118">Kansion aktiviteetit</span><span class="sxs-lookup"><span data-stu-id="72503-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="72503-119">Pyyntöaktiviteettien jakaminen ja käyttäminen</span><span class="sxs-lookup"><span data-stu-id="72503-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="72503-120">Synkronointiaktiviteetit</span><span class="sxs-lookup"><span data-stu-id="72503-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="72503-121">Sivuston hallintatoiminnot</span><span class="sxs-lookup"><span data-stu-id="72503-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="72503-122">Lisätietoja näiden tapahtumien noutamisesta on kohdassa [Valvontalokista etsiminen](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="72503-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
