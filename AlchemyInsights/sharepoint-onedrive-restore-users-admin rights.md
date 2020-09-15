---
title: Käyttö estetty-viestien vian määritys OneDrive for Business-sivustossa
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670613"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="2b12a-102">Käyttö estetty-viestien vian määritys OneDrive for Business-sivustossa</span><span class="sxs-lookup"><span data-stu-id="2b12a-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="2b12a-103">Tämä ongelma ilmenee useimmiten silloin, kun käyttäjä poistetaan ja luodaan uudelleen käyttäen samaa käyttäjän päänimeä (UPN).</span><span class="sxs-lookup"><span data-stu-id="2b12a-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="2b12a-104">Uusi tili luodaan käyttämällä toista PUID (Passport Unique ID)-arvoa.</span><span class="sxs-lookup"><span data-stu-id="2b12a-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="2b12a-105">Kun käyttäjä yrittää käyttää sivustokokoelmaa tai OneDrivea, käyttäjällä on virheellinen PUID.</span><span class="sxs-lookup"><span data-stu-id="2b12a-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="2b12a-106">Toinen skenaario sisältää hakemisto synkronoinnin Active Directoryn organisaatio yksikön (OU) kanssa.</span><span class="sxs-lookup"><span data-stu-id="2b12a-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="2b12a-107">Jos käyttäjä on jo kirjautunut SharePointiin ja siirtyy sitten toiseen organisaatio yksikköön ja on siirretty SharePointiin, ongelma saattaa ilmetä.</span><span class="sxs-lookup"><span data-stu-id="2b12a-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="2b12a-108">Voit korjata ongelman palauttamalla alkuperäisen UPN:N artikkelin ohjeiden mukaisesti ja [palauttamalla käyttäjän Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)-sovelluksessa.</span><span class="sxs-lookup"><span data-stu-id="2b12a-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="2b12a-109">Jos et pysty palauttamaan alkuperäistä käyttäjää, sinun on poistettava vanha käyttäjä OneDrive-sivustosta noudattamalla näitä ohjeita, [poistamalla käyttäjä käyttäjä tieto luettelosta]().</span><span class="sxs-lookup"><span data-stu-id="2b12a-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="2b12a-110">Kun tämä on tehty, voit tarkistaa, että käyttäjällä on järjestelmänvalvojan oikeudet OneDrive-sivustoon, noudattamalla ohjeita, jotka koskevat [järjestelmänvalvojan lisäämistä käyttäjän OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles) -palveluun.</span><span class="sxs-lookup"><span data-stu-id="2b12a-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="2b12a-111">Lisä tietoja käyttö oikeus tasoista on artikkelissa tietoja [SharePointin käyttö oikeus tasoista](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="2b12a-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
