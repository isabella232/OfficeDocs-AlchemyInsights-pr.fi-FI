---
title: Vianmääritys Access estetty viestien OneDrive Business sivustot
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: d47ce80bdd07a25d9724057edf0289808a00a3db
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232521"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="37706-102">Vianmääritys Access estetty viestien OneDrive Business sivustot</span><span class="sxs-lookup"><span data-stu-id="37706-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="37706-103">Tämä ongelma ilmenee usein, kun käyttäjä poistetaan ja luodaan uudelleen sama käyttäjätunnus (UPN) kanssa.</span><span class="sxs-lookup"><span data-stu-id="37706-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="37706-104">Uusi tili on luotu käyttämällä eri PUID (yksilöllisen Passport-tunnus)-arvoa.</span><span class="sxs-lookup"><span data-stu-id="37706-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="37706-105">Kun käyttäjä yrittää käyttää sivustokokoelman tai niiden OneDrive, käyttäjällä on virheellinen PUID.</span><span class="sxs-lookup"><span data-stu-id="37706-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="37706-106">Toinen tilanne liittyy directory-synkronointia Active Directoryn organisaatioyksikössä (OU).</span><span class="sxs-lookup"><span data-stu-id="37706-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="37706-107">Jos käyttäjät ovat jo kirjautuneena SharePoint-ovat siirretään eri OU ja SharePointin kanssa resynced, he saattavat kohdata tämän ongelman.</span><span class="sxs-lookup"><span data-stu-id="37706-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="37706-108">Voit ratkaista tämän ongelman olisi palauttaa alkuperäisen UPN kanssa artikkelin,[Palauta Office 365-käyttäjä](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="37706-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="37706-109">Jos et pysty palauttamaan alkuperäinen käyttäjä poistaa vanhan käyttäjän OneDrive-sivuston, näillä ohjeilla, [Poista käyttäjä-käyttäjätietojen luettelossa]().</span><span class="sxs-lookup"><span data-stu-id="37706-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="37706-110">Tämän jälkeen voit tarkistaa käyttäjällä on admin oikeudet OneDrive-sivuston [admin Lisää käyttäjän, käyttäjän OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive) ohjeiden mukaisesti</span><span class="sxs-lookup"><span data-stu-id="37706-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="37706-111">Lisätietoja käyttöoikeustasoista on artikkelissa, [ymmärtäminen käyttöoikeustasoja SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="37706-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
