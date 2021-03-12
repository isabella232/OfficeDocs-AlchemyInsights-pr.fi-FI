---
title: Tätä sivustoa ei voi saavuttaa – virhe yritettäessä käyttää SharePoint-sivustoa selaimesta tai Teamsista
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005378"
- "9266"
ms.openlocfilehash: 451544fb85522e0eececc9274825805699685ee9
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744983"
---
# <a name="this-site-cant-be-reached-error-when-trying-to-access-sharepoint-site-from-browser-or-teams"></a><span data-ttu-id="079f6-102">Tämä sivusto ei ole saavutettu -virhe, kun yrität käyttää SharePoint-sivustoa selaimesta tai Teamsista</span><span class="sxs-lookup"><span data-stu-id="079f6-102">“This site can’t be reached” error when trying to access SharePoint site from browser or Teams</span></span>

<span data-ttu-id="079f6-103">Käyttäjät saattavat saada "Tätä sivustoa ei voi saavuttaa" -virheilmoituksen, kun he yrittävät käyttää SharePoint-sivustoa selaimessa tai Teamsissa.</span><span class="sxs-lookup"><span data-stu-id="079f6-103">Users might receive "This site can't be reached" error when trying to access SharePoint site from browser or Teams.</span></span> 

<span data-ttu-id="079f6-104">Voit ratkaista ongelman näin:</span><span class="sxs-lookup"><span data-stu-id="079f6-104">To resolve this issue:</span></span> 

1. <span data-ttu-id="079f6-105">Tarkista, onko aloitussivu roskakorissa vai toisen vaiheen roskakorissa, ja palauta sivu.</span><span class="sxs-lookup"><span data-stu-id="079f6-105">Check if the home page is in Recycle bin or second-stage recycle bin and restore the page.</span></span>

<span data-ttu-id="079f6-106">**Esimerkki suorasta URL-osoitteesta roskakoriin:**https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span><span class="sxs-lookup"><span data-stu-id="079f6-106">**Sample direct URL to recycle bin**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span></span>

1. <span data-ttu-id="079f6-107">Jos aloitussivu poistetaan pysyvästi roskakorista, luo uusi sivustosivu Sivuston sivut -kirjastosta ja tee siitä aloitussivu.</span><span class="sxs-lookup"><span data-stu-id="079f6-107">If the home page is permanently removed from the recycle bin, create a new site page from the Site Pages library and make it a homepage.</span></span> 

<span data-ttu-id="079f6-108">**Suoran URL-osoitteen esimerkki:**https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span><span class="sxs-lookup"><span data-stu-id="079f6-108">**Sample direct URL**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span></span>