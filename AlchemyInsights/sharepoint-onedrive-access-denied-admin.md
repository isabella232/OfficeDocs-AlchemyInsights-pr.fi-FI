---
title: Käyttö estetty-viestien vian määritys
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767659"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="9c4c9-102">Käyttö estetty-viestien vian määritys SharePoint/OneDrive-hallinta keskuksessa</span><span class="sxs-lookup"><span data-stu-id="9c4c9-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="9c4c9-103">Jos vastaanotat käyttö estetty-viestin, kun yrität siirtyä SharePoint/OneDrive-hallinta keskukseen, varmista, että määrität [käyttäjälle käyttö oikeuden](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="9c4c9-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="9c4c9-104">Jos käyttäjällä on käyttö oikeus, Varmista myös, että [hänelle on määritetty järjestelmänvalvojan rooli](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , joka voi käyttää hallinta keskuksia.</span><span class="sxs-lookup"><span data-stu-id="9c4c9-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="9c4c9-105">Tämä ongelma voi ilmetä myös silloin, kun käyttäjä poistetaan ja luodaan uudelleen käyttäen samaa käyttäjän päänimeä (UPN).</span><span class="sxs-lookup"><span data-stu-id="9c4c9-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="9c4c9-106">Uusi tili luodaan käyttämällä toista PUID (Passport Unique ID)-arvoa.</span><span class="sxs-lookup"><span data-stu-id="9c4c9-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="9c4c9-107">Kun käyttäjä yrittää käyttää sivustokokoelmaa tai OneDrivea, käyttäjällä on virheellinen PUID.</span><span class="sxs-lookup"><span data-stu-id="9c4c9-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="9c4c9-108">Toinen skenaario sisältää hakemisto synkronoinnin Active Directoryn organisaatio yksikön (OU) kanssa.</span><span class="sxs-lookup"><span data-stu-id="9c4c9-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="9c4c9-109">Jos käyttäjä on jo kirjautunut SharePointiin ja siirtyy sitten toiseen organisaatio yksikköön ja on siirretty SharePointiin, ongelma saattaa ilmetä.</span><span class="sxs-lookup"><span data-stu-id="9c4c9-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="9c4c9-110">Voit korjata ongelman palauttamalla alkuperäisen UPN:N artikkelin ohjeiden mukaisesti ja [palauttamalla käyttäjän Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)-sovelluksessa.</span><span class="sxs-lookup"><span data-stu-id="9c4c9-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="9c4c9-111">Huomautus: Jos OneDrive-tai SharePoint-hallinta keskus ei ole käytettävissä useille käyttäjille, joilla on aiemmin ollut käyttö oikeus, kyseessä saattaa olla tilapäinen palvelu ongelma.</span><span class="sxs-lookup"><span data-stu-id="9c4c9-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="9c4c9-112">[Tarkista palvelun kunnon koonti näyttö](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="9c4c9-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


