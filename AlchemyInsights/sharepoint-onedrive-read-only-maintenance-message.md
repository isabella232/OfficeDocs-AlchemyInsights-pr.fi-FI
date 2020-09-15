---
title: Ylläpito viestin vain luku-tilassa, kun yrität käyttää SharePointia tai OneDrivea
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670829"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="f21d1-102">Ylläpito viestin vain luku-tilassa, kun yrität käyttää SharePointia tai OneDrivea</span><span class="sxs-lookup"><span data-stu-id="f21d1-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="f21d1-103">Käyttäjät voivat saada **vain luku-tilassa olevan ylläpito** viestin, kun he yrittävät käyttää SharePointia tai OneDrivea jossakin seuraavista tilanteista.</span><span class="sxs-lookup"><span data-stu-id="f21d1-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="f21d1-104">Suunniteltu tai aktiivinen huolto toiminto.</span><span class="sxs-lookup"><span data-stu-id="f21d1-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="f21d1-105">Tarkista ne siirtymällä [viesti keskukseen](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="f21d1-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="f21d1-106">Erittäin tärkeä, aktiivinen palvelu häiriö, joka saattaa olla käynnissä.</span><span class="sxs-lookup"><span data-stu-id="f21d1-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="f21d1-107">Tarkista kaikki varoitukset/häiriöt siirtymällä kohtaan [palvelun kunto](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="f21d1-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="f21d1-108">Pieni automaattisen paranemisen palautus skenaario, joka voi johtua sellaisista palvelimista, jotka saattavat kestää alle 30 minuuttia.</span><span class="sxs-lookup"><span data-stu-id="f21d1-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="f21d1-109">Näiden vähäisten palautuksista ei ole viesti keskusta tai palvelun kunnon viestejä, mutta sinun pitäisi palata normaaliin hyvin pian.</span><span class="sxs-lookup"><span data-stu-id="f21d1-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="f21d1-110">Olemme havainneet, että yksi edellä mainituista kolmesta skenaarioista on ollut syynä ja että palvelu on palautettu, mutta käyttäjät-selaimen väli muistia ei ole selvitetty.</span><span class="sxs-lookup"><span data-stu-id="f21d1-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="f21d1-111">Yritä tyhjentää selaimen väli muisti ennen sivustoon siirtymistä.</span><span class="sxs-lookup"><span data-stu-id="f21d1-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="f21d1-112">Valitse Microsoft Edge-selaimessa **Asetukset**ja valitse sitten **tieto suoja ja suojaus**.</span><span class="sxs-lookup"><span data-stu-id="f21d1-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="f21d1-113">Valitse **Tyhjennä selaaminen**-kohdassa **Valitse, mitä haluat tyhjentää**.</span><span class="sxs-lookup"><span data-stu-id="f21d1-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="f21d1-114">Valitse **eväs teet ja tallennetut sivuston tiedot**ja valitse **Tyhjennä**.</span><span class="sxs-lookup"><span data-stu-id="f21d1-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="f21d1-115">Nämä vaiheet voivat vaihdella, kun käytät muita selaimia, kuten Mozilla Firefoxia tai Google Chromea.</span><span class="sxs-lookup"><span data-stu-id="f21d1-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="f21d1-116">Toinen vaihto ehto on avata SharePoint-sivusto tai OneDrive uudessa InPrivate-ikkunassa.</span><span class="sxs-lookup"><span data-stu-id="f21d1-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>