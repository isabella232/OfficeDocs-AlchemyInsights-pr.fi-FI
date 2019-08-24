---
title: Vain luku-ylläpito tulee näyttöön, kun yrität käyttää SharePoint- tai OneDrive
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620720"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="61ca1-102">Vain luku-ylläpito tulee näyttöön, kun yrität käyttää SharePoint- tai OneDrive</span><span class="sxs-lookup"><span data-stu-id="61ca1-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="61ca1-103">Käyttäjät saattavat saada **Ylläpito vain luku -** viestin, kun yrität käyttää SharePoint- tai OneDrive seuraavissa tilanteissa.</span><span class="sxs-lookup"><span data-stu-id="61ca1-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="61ca1-104">Suunniteltu tai aktiivinen huoltotoimet.</span><span class="sxs-lookup"><span data-stu-id="61ca1-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="61ca1-105">Tarkista ne siirtymällä [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="61ca1-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="61ca1-106">Suuren prioriteetin aktiivisen palvelun ajankohta, joka on esiintyvä.</span><span class="sxs-lookup"><span data-stu-id="61ca1-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="61ca1-107">Tarkista siirtymällä [Terveyden huollon](https://portal.office.com/adminportal/home#/servicehealth)tiedotteiden ja tapahtumat.</span><span class="sxs-lookup"><span data-stu-id="61ca1-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="61ca1-108">Pieni auto kenties recovery skenaario, joka saattaa toimi koska odottamattomia tapahtumia palvelimissa, jotka saattavat kestää alle 30 minuuttia tai niin.</span><span class="sxs-lookup"><span data-stu-id="61ca1-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="61ca1-109">On Message Center ei ole tai palvelu terveyden kirjaa nämä pienet saantotiedot mutta pitäisi olla takaisin normaaliksi on hyvin pian.</span><span class="sxs-lookup"><span data-stu-id="61ca1-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="61ca1-110">Vain muutamia kertoja olemme havaitaan jokin edellä mainitut kolme tilanteita on ollut syy, ja palvelu on palautettu mutta käyttäjien selaimen välimuisti ei ole vielä tyhjennetty.</span><span class="sxs-lookup"><span data-stu-id="61ca1-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="61ca1-111">Yritä tyhjentää selaimen välimuisti ennen sivuston navigointi.</span><span class="sxs-lookup"><span data-stu-id="61ca1-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="61ca1-112">Microsoft Edge-selaimessa Valitse **asetukset**ja valitse sitten **Tietosuoja- ja**.</span><span class="sxs-lookup"><span data-stu-id="61ca1-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="61ca1-113">Valitse **Poista selaaminen**, **Valitse mitä haluat poistaa**.</span><span class="sxs-lookup"><span data-stu-id="61ca1-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="61ca1-114">**Evästeet ja tallennetun Web-sivun tiedot**ja valitse **Poista**.</span><span class="sxs-lookup"><span data-stu-id="61ca1-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="61ca1-115">Nämä vaiheet saattavat vaihdella muissa selaimissa, kuten Mozilla Firefox tai Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="61ca1-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="61ca1-116">Avaa uusi InPrivate-ikkunassa SharePoint-sivuston tai OneDrive olisi toinen vaihtoehto.</span><span class="sxs-lookup"><span data-stu-id="61ca1-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>