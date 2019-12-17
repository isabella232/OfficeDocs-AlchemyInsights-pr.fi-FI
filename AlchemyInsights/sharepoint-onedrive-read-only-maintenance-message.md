---
title: Vain luku-ylläpito sanoma yritettäessä käyttää SharePointia tai OneDrivea
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051278"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="93eb7-102">Vain luku-ylläpito sanoma yritettäessä käyttää SharePointia tai OneDrivea</span><span class="sxs-lookup"><span data-stu-id="93eb7-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="93eb7-103">Käyttäjät saattavat saada **vain luku-tilassa olevan ylläpito** sanoman yrittäessään käyttää SharePointia tai OneDrivea jossakin seuraavista tilanteista.</span><span class="sxs-lookup"><span data-stu-id="93eb7-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="93eb7-104">Suunniteltua tai aktiivista kunnossapitoaktiviteettia.</span><span class="sxs-lookup"><span data-stu-id="93eb7-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="93eb7-105">Tarkista ne siirtymällä [viesti keskukseen](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="93eb7-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="93eb7-106">Erittäin tärkeä aktiivinen palvelu tapahtuma, joka saattaa olla tapahtumassa.</span><span class="sxs-lookup"><span data-stu-id="93eb7-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="93eb7-107">Tarkista mahdolliset neuvot/tapahtumat siirtymällä [palvelun terveyteen](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="93eb7-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="93eb7-108">Pieni auto-Healing elpyminen skenaario, joka voi tapahtua, koska odottamattomia tapahtumia palvelimet, jotka voivat kestää alle 30 min tai niin.</span><span class="sxs-lookup"><span data-stu-id="93eb7-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="93eb7-109">Näitä vähäisiä takaisinperintöjä varten ei ole Message Center-tai Service Health-viestejä, mutta sinun pitäisi palata normaaliksi hyvin pian.</span><span class="sxs-lookup"><span data-stu-id="93eb7-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="93eb7-110">Hyvin harvoissa tapa uksissa havaitsimme, että yksi edellä mainituista kolmesta skenaariosta on ollut syynä, ja palvelu on palautettu, mutta käyttäjien selaimen väli muistia ei ole selvitetty.</span><span class="sxs-lookup"><span data-stu-id="93eb7-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="93eb7-111">Yritä tyhjentää selaimen väli muisti ennen navigointia sivustoon.</span><span class="sxs-lookup"><span data-stu-id="93eb7-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="93eb7-112">Valitse Microsoft Edge-selaimessa **Asetukset**ja valitse sitten **yksityisyys ja suojaus**.</span><span class="sxs-lookup"><span data-stu-id="93eb7-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="93eb7-113">Valitse **Tyhjennä selaus**-kohdassa Valitse, **mitä haluat tyhjentää**.</span><span class="sxs-lookup"><span data-stu-id="93eb7-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="93eb7-114">Valitse **eväs teet ja tallennetut verkkosivustotiedot**ja valitse **Tyhjennä**.</span><span class="sxs-lookup"><span data-stu-id="93eb7-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="93eb7-115">Nämä vaiheet saattavat vaihdella käytettäessä muita selaimia, kuten Mozilla Firefox tai Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="93eb7-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="93eb7-116">Toinen vaihto ehto olisi avata SharePoint-sivusto tai OneDrive uuteen InPrivate-ikkunaan.</span><span class="sxs-lookup"><span data-stu-id="93eb7-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>