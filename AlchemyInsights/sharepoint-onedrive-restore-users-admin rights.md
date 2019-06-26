---
title: Vianmääritys Access estetty viestien OneDrive Business sivustot
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: b394cc1441187133d8829cfc5fb0c1edbd71fd96
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223421"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="1dbdc-102">Vianmääritys Access estetty viestien OneDrive Business sivustot</span><span class="sxs-lookup"><span data-stu-id="1dbdc-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="1dbdc-103">Tämä ongelma ilmenee usein, kun käyttäjä poistetaan ja luodaan uudelleen sama käyttäjätunnus (UPN) kanssa.</span><span class="sxs-lookup"><span data-stu-id="1dbdc-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="1dbdc-104">Uusi tili on luotu käyttämällä eri PUID (yksilöllisen Passport-tunnus)-arvoa.</span><span class="sxs-lookup"><span data-stu-id="1dbdc-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="1dbdc-105">Kun käyttäjä yrittää käyttää sivustokokoelman tai niiden OneDrive, käyttäjällä on virheellinen PUID.</span><span class="sxs-lookup"><span data-stu-id="1dbdc-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="1dbdc-106">Toinen tilanne liittyy directory-synkronointia Active Directoryn organisaatioyksikössä (OU).</span><span class="sxs-lookup"><span data-stu-id="1dbdc-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="1dbdc-107">Jos käyttäjät ovat jo kirjautuneena SharePoint-ovat siirretään eri OU ja SharePointin kanssa resynced, he saattavat kohdata tämän ongelman.</span><span class="sxs-lookup"><span data-stu-id="1dbdc-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="1dbdc-108">Voit ratkaista tämän ongelman olisi palauttaa alkuperäisen UPN kanssa artikkelin,[Palauta Office 365-käyttäjä](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="1dbdc-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="1dbdc-109">Tämän jälkeen voit tarkistaa käyttäjällä on admin oikeudet OneDrive-sivuston [admin Lisää käyttäjän, käyttäjän OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive) ohjeiden mukaisesti</span><span class="sxs-lookup"><span data-stu-id="1dbdc-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="1dbdc-110">Lisätietoja käyttöoikeustasoista on artikkelissa, [ymmärtäminen käyttöoikeustasoja SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="1dbdc-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
