---
title: OneDrive for Business -sivustojen käytön estämien viestien vianmääritys
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511181"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="0c4ef-102">OneDrive for Business -sivustojen käytön estämien viestien vianmääritys</span><span class="sxs-lookup"><span data-stu-id="0c4ef-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="0c4ef-103">Tämä ongelma ilmenee useimmiten, kun käyttäjä poistetaan ja luodaan uudelleen samalla käyttäjänimellä (UPN).</span><span class="sxs-lookup"><span data-stu-id="0c4ef-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="0c4ef-104">Uusi tili luodaan käyttämällä toista PUID (Passport Unique ID) -arvoa.</span><span class="sxs-lookup"><span data-stu-id="0c4ef-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="0c4ef-105">Kun käyttäjä yrittää käyttää sivustokokoelmaa tai OneDrivea, käyttäjällä on virheellinen PUID-tunnus.</span><span class="sxs-lookup"><span data-stu-id="0c4ef-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="0c4ef-106">Toinen skenaario koskee hakemistosynkronointia Active Directory -organisaatioyksikön kanssa.</span><span class="sxs-lookup"><span data-stu-id="0c4ef-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="0c4ef-107">Jos käyttäjät ovat jo kirjautuneet SharePointiin ja siirtyvät sitten toiseen organisaatioyksikköön ja synkronoivat sharepointin uudelleen, he saattavat kohdata tämän ongelman.</span><span class="sxs-lookup"><span data-stu-id="0c4ef-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="0c4ef-108">Voit ratkaista tämän ongelman palauttamalla alkuperäisen UPN-numeron artikkelin ohjeiden mukaisesti, [jotka on tarkoitettu käyttäjän palauttamiseen Microsoft 365 :ssä](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="0c4ef-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="0c4ef-109">Jos et pysty palauttamaan alkuperäistä käyttäjää, poista vanha käyttäjä OneDrive-sivustosta seuraavasti, [poista käyttäjä käyttäjätietoluettelosta]().</span><span class="sxs-lookup"><span data-stu-id="0c4ef-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="0c4ef-110">Kun tämä on tehty, voit varmistaa, että käyttäjällä on järjestelmänvalvojan oikeudet OneDrive-sivustoon, noudattamalla käyttäjän [OneDrive-järjestelmänvalvojan käyttäjien järjestelmänvalvojan oikeuksien lisäämistä](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="0c4ef-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="0c4ef-111">Lisätietoja käyttöoikeustasoista on artikkelissa [Tietoja SharePointin käyttöoikeustasoista](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="0c4ef-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
