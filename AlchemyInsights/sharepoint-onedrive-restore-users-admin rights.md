---
title: OneDrive for Business-sivustojen käyttö estetty-sanomien vian määritys
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/15/2019
ms.locfileid: "37766708"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="a223e-102">OneDrive for Business-sivustojen käyttö estetty-sanomien vian määritys</span><span class="sxs-lookup"><span data-stu-id="a223e-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="a223e-103">Tämä ongelma ilmenee useimmin, kun käyttäjä poistetaan ja luodaan uudelleen samalla käyttäjä nimellä (UPN).</span><span class="sxs-lookup"><span data-stu-id="a223e-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="a223e-104">Uusi tili luodaan käyttämällä eri PUID (Passport Unique ID)-arvoa.</span><span class="sxs-lookup"><span data-stu-id="a223e-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="a223e-105">Kun käyttäjä yrittää käyttää sivustokokoelmaa tai OneDrivea, käyttäjällä on väärä PUID-tunnus.</span><span class="sxs-lookup"><span data-stu-id="a223e-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="a223e-106">Toinen skenaario koskee hakemiston synkronointia Active Directory-organisaatio yksikön (OU) kanssa.</span><span class="sxs-lookup"><span data-stu-id="a223e-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="a223e-107">Jos käyttäjät ovat jo kirjauduneet sisään SharePointiin ja ne siirretään toiseen kohteeseen ja synkronoidaan SharePointin kanssa, ongelma saattaa ilmetä.</span><span class="sxs-lookup"><span data-stu-id="a223e-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="a223e-108">Voit ratkaista tämän ongelman palauttamalla alkuperäisen UPN artikkelin vaiheet, [Palauta käyttäjä Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="a223e-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="a223e-109">Jos et pysty palauttamaan alkuperäistä käyttäjää, poista vanha käyttäjä OneDrive-sivustosta näiden vaiheiden avulla, [Poista käyttäjä käyttäjän tiedot-luettelosta]().</span><span class="sxs-lookup"><span data-stu-id="a223e-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="a223e-110">Kun tämä on tehty, voit varmistaa, että käyttäjällä on järjestelmänvalvojan oikeudet OneDrive-sivustoon noudattamalla ohjeita, jotka [lisäävät järjestelmänvalvojan tiedot käyttäjän OneDriveen](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="a223e-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="a223e-111">Lisä tietoja käyttö oikeus tasoista on artikkelissa [SharePoint-käyttö oikeus tasojen ymmärtäminen](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="a223e-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
