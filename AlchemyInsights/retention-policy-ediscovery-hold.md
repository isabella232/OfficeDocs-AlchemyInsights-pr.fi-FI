---
title: 2609-säilyttäminen-tai-eDiscovery-Hold
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
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994060"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="9e6aa-102">Kohteita ei voi poistaa SharePoint Onlinessa tai OneDrive for Businessissa</span><span class="sxs-lookup"><span data-stu-id="9e6aa-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="9e6aa-103">Sinä tai käyttäjät emme ehkä voi poistaa kohteita SharePoint Onlinessa tai OneDrive for Businessissa, koska säilytys käytäntöä, säilytys otsikkoa tai eDiscovery-pito toimintoa käytetään OneDrive-sivuston SharePointiin tai tiettyyn kohteeseen.</span><span class="sxs-lookup"><span data-stu-id="9e6aa-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="9e6aa-104">Tämä ei kuitenkaan voi poistaa asia kirjaa, asia kirjan versiota, kansiota, asiakirja kirjastoa, luetteloa, sovellusta, sivustoa tai sivustokokoelmaa.</span><span class="sxs-lookup"><span data-stu-id="9e6aa-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="9e6aa-105">Seuraavassa on joitakin esimerkkejä virhe ilmoituksista, jotka saatat saada, jos yrität poistaa säilytettävien kohteiden:</span><span class="sxs-lookup"><span data-stu-id="9e6aa-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="9e6aa-106">"Tätä sivustoa ei voi poistaa, koska se sisältyy eDiscovery Hold-tai säilytys käytäntöön"</span><span class="sxs-lookup"><span data-stu-id="9e6aa-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="9e6aa-107">"Tämän sivuston yhteensopivuus käytäntö on määritetty estämään poistaminen"</span><span class="sxs-lookup"><span data-stu-id="9e6aa-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="9e6aa-108">"Yhteensopivuus käytäntö estää tällä hetkellä sivuston poistamisen"</span><span class="sxs-lookup"><span data-stu-id="9e6aa-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="9e6aa-109">"Tätä sivustokokoelmaa ei voi poistaa, koska se sisältää eDiscovery Hold-tai säilytys käytäntöön sisältyviä sivustoja."</span><span class="sxs-lookup"><span data-stu-id="9e6aa-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="9e6aa-110">"Sinun on poistettava kaikki tämän kansion kohteet ennen kansion poistamista"</span><span class="sxs-lookup"><span data-stu-id="9e6aa-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="9e6aa-111">"Tämän kohteen versioita ei voi poistaa, koska se on Hold-tai säilytys käytännöllä"</span><span class="sxs-lookup"><span data-stu-id="9e6aa-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="9e6aa-112">Kohdetta ei voi poistaa Hold-aikana</span><span class="sxs-lookup"><span data-stu-id="9e6aa-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="9e6aa-113">"Tähän kohteeseen kohdistettu selite estää sen muokkaamisen tai poistamisen"</span><span class="sxs-lookup"><span data-stu-id="9e6aa-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="9e6aa-114">"Luetteloa ei voi poistaa Hold-tai säilytys käytännöllä"</span><span class="sxs-lookup"><span data-stu-id="9e6aa-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="9e6aa-115">"Luetteloa ei voi poistaa, jos se on estetty tai jos siihen sovelletaan säilytys käytäntöä"</span><span class="sxs-lookup"><span data-stu-id="9e6aa-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="9e6aa-116">Jos haluat poistaa kohteita jossakin näistä skenaarioista, säilytys käytäntö, säilytys etiketti tai eDiscovery-pito on poistettava (tai sivusto on jätettävä säilytys käytännön ulkopuolelle).</span><span class="sxs-lookup"><span data-stu-id="9e6aa-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="9e6aa-117">Sinun on joko poistettava käytöstä tai suljettava pois tämä ongelma aiheuttava pito.</span><span class="sxs-lookup"><span data-stu-id="9e6aa-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="9e6aa-118">Kun säilytys käytäntö tai pito on poistettu, muutos tulee voimaan 24 tunnin kuluttua.</span><span class="sxs-lookup"><span data-stu-id="9e6aa-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="9e6aa-119">Lisä tietoja erilaisista säilytys-ja pito ominaisuuksista, joita voidaan käyttää SharePoint-sivustoissa ja OneDrive-tileissä, on seuraavissa ohje aiheissa:</span><span class="sxs-lookup"><span data-stu-id="9e6aa-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="9e6aa-120">Yleiskatsaus säilytys käytäntöihin</span><span class="sxs-lookup"><span data-stu-id="9e6aa-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="9e6aa-121">Yleiskatsaus säilytys tarroihin</span><span class="sxs-lookup"><span data-stu-id="9e6aa-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="9e6aa-122">Hallitse pidot Advanced eDiscovery-kohteessa</span><span class="sxs-lookup"><span data-stu-id="9e6aa-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="9e6aa-123">eDiscovery omistaa</span><span class="sxs-lookup"><span data-stu-id="9e6aa-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="9e6aa-124">Vanhojen sivustojen sulkemis-ja poisto käytännöt</span><span class="sxs-lookup"><span data-stu-id="9e6aa-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
