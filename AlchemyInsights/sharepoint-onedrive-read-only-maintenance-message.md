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
ms.openlocfilehash: cc232fba6f502e2b6f282a8c1a1e29221e36b70d
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840512"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="2e4e6-102">Vain luku-ylläpito tulee näyttöön, kun yrität käyttää SharePoint- tai OneDrive</span><span class="sxs-lookup"><span data-stu-id="2e4e6-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="2e4e6-103">Käyttäjät saattavat saada **Ylläpito vain luku -** viestin, kun yrität käyttää SharePoint- tai OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2e4e6-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive.</span></span>  <span data-ttu-id="2e4e6-104">Jos näin on, tarkista, onko aktiivisen ylläpidon käynnistämien että vuokralaisen siirtymällä [viestikeskuksesta](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="2e4e6-104">If so, check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span> <span data-ttu-id="2e4e6-105">Varmista myös, että [Terveyden huollon](https://portal.office.com/adminportal/home#/servicehealth) koontinäytön tiedotteiden ja tapahtumat, jotka on määrä tarkistaa.</span><span class="sxs-lookup"><span data-stu-id="2e4e6-105">Also, make sure to check the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) dashboard to check for any advisories/incidents that may be occurring.</span></span>

<span data-ttu-id="2e4e6-106">Jos ole Message Center- tai terveyden huollon dashboard on mainita mitään tietoja nykyisen Kunnossapito, että vuokralaisen, ongelma saattaa johtua selaimen välimuisti ongelma.</span><span class="sxs-lookup"><span data-stu-id="2e4e6-106">If neither the Message Center or Service Health dashboard have noted anything about current maintenance for your tenant, this may be a browser caching issue.</span></span>

<span data-ttu-id="2e4e6-107">Yritä tyhjentää selaimen välimuisti ennen sivuston navigointi.</span><span class="sxs-lookup"><span data-stu-id="2e4e6-107">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="2e4e6-108">Microsoft Edge-selaimessa Valitse **asetukset**ja valitse sitten **Tietosuoja- ja**.</span><span class="sxs-lookup"><span data-stu-id="2e4e6-108">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="2e4e6-109">Valitse **Poista selaaminen**, **Valitse mitä haluat poistaa**.</span><span class="sxs-lookup"><span data-stu-id="2e4e6-109">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="2e4e6-110">**Evästeet ja tallennetun Web-sivun tiedot**ja valitse **Poista**.</span><span class="sxs-lookup"><span data-stu-id="2e4e6-110">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="2e4e6-111">Nämä vaiheet saattavat vaihdella muissa selaimissa, kuten Mozilla Firefox tai Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="2e4e6-111">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="2e4e6-112">Avaa uusi InPrivate-ikkunassa SharePoint-sivuston tai OneDrive olisi toinen vaihtoehto.</span><span class="sxs-lookup"><span data-stu-id="2e4e6-112">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>