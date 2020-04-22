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
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741962"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="12700-102">SharePointin ja OneDriven valvontalokit</span><span class="sxs-lookup"><span data-stu-id="12700-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="12700-103">SharePointin perinteiset valvontalokit</span><span class="sxs-lookup"><span data-stu-id="12700-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="12700-104">SPO:n vanha valvonta siirrettiin Yhdistettyyn valvontalokiin (UAL).</span><span class="sxs-lookup"><span data-stu-id="12700-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="12700-105">Kaikki spo:n vanhat auditointiraportit toimitetaan nyt UAL:n kautta ja vanhat auditointisignaalit on siirretty UAL:hen.</span><span class="sxs-lookup"><span data-stu-id="12700-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="12700-106">Tärkeimmät muutokset:</span><span class="sxs-lookup"><span data-stu-id="12700-106">Key changes:</span></span>

* <span data-ttu-id="12700-107">Trimmaus ei ole käytettävissä ominaisuutena.</span><span class="sxs-lookup"><span data-stu-id="12700-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="12700-108">Tiettyjen valvottavien tapahtumien valitseminen ei ole käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="12700-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="12700-109">Tässä [asiakirjassa](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) on täydellinen luettelo oletusarvoisesti käytettävissä olevista valvotuista tapahtumista.</span><span class="sxs-lookup"><span data-stu-id="12700-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="12700-110">**Mukautetut raportit** -kohdan **Sijainti-vaihtoehto** ei ole käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="12700-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="12700-111">**Asiakirjojen avaaminen tai lataaminen** -vaihtoehto ei ole käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="12700-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="12700-112">Sivustokokoelman valvonta-asetusten määrittäminen</span><span class="sxs-lookup"><span data-stu-id="12700-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="12700-113">SharePointin ja OneDriven nykyaikaiset yhdistetyt valvontalokit yhteensopivuudesta</span><span class="sxs-lookup"><span data-stu-id="12700-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="12700-114">Yhdistetyn valvonnan kirjaamisen ottaminen käyttöön tai poistaminen käytöstä</span><span class="sxs-lookup"><span data-stu-id="12700-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="12700-115">Lisämäärityksiä ei tarvita SharePointissa tai OneDrivessa.</span><span class="sxs-lookup"><span data-stu-id="12700-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="12700-116">Tarkista tiedostojen, kansioiden, käyttäjien ja käyttöoikeuksien toiminta valvontalokihaun avulla:</span><span class="sxs-lookup"><span data-stu-id="12700-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="12700-117">Tiedostojen ja sivujen aktiviteetit</span><span class="sxs-lookup"><span data-stu-id="12700-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="12700-118">Kansion toiminnot</span><span class="sxs-lookup"><span data-stu-id="12700-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="12700-119">Jakamis- ja käyttöoikeuspyyntöaktiviteetit</span><span class="sxs-lookup"><span data-stu-id="12700-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="12700-120">Synkronointiaktiviteetit</span><span class="sxs-lookup"><span data-stu-id="12700-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="12700-121">Sivuston hallintatoiminnot</span><span class="sxs-lookup"><span data-stu-id="12700-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="12700-122">Lisätietoja näiden tapahtumien noutamisesta on kohdassa [Haku valvontalokista](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="12700-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
