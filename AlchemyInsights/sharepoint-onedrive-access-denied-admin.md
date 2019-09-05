---
title: Käyttö estetty-sanomien vian määritys
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751273"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="44ba2-102">SharePoint/OneDrive-hallinta keskuksen käyttö estetty-viestien vian määritys</span><span class="sxs-lookup"><span data-stu-id="44ba2-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="44ba2-103">Jos saat käyttö estetty-sanoman yritettäessä selata SharePoint/OneDrive-hallinta keskukseen, varmista, että määrität [käyttäjälle](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)käyttö oikeuden.</span><span class="sxs-lookup"><span data-stu-id="44ba2-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="44ba2-104">Jos käyttäjällä on käyttö oikeus, Varmista myös, että heille on [määritetty järjestelmänvalvojan rooli](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , joka voi käyttää hallinta keskuksia.</span><span class="sxs-lookup"><span data-stu-id="44ba2-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="44ba2-105">Tämä ongelma voi ilmetä myös, kun käyttäjä poistetaan ja luodaan uudelleen samalla käyttäjä nimellä (UPN).</span><span class="sxs-lookup"><span data-stu-id="44ba2-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="44ba2-106">Uusi tili luodaan käyttämällä eri PUID (Passport Unique ID)-arvoa.</span><span class="sxs-lookup"><span data-stu-id="44ba2-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="44ba2-107">Kun käyttäjä yrittää käyttää sivustokokoelmaa tai OneDrivea, käyttäjällä on väärä PUID-tunnus.</span><span class="sxs-lookup"><span data-stu-id="44ba2-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="44ba2-108">Toinen skenaario koskee hakemiston synkronointia Active Directory-organisaatio yksikön (OU) kanssa.</span><span class="sxs-lookup"><span data-stu-id="44ba2-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="44ba2-109">Jos käyttäjät ovat jo kirjauduneet sisään SharePointiin ja ne siirretään toiseen kohteeseen ja synkronoidaan SharePointin kanssa, ongelma saattaa ilmetä.</span><span class="sxs-lookup"><span data-stu-id="44ba2-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="44ba2-110">Voit ratkaista tämän ongelman palauttamalla alkuperäisen käyttäjä tieto järjestelmän artikkelin ohjeiden mukaisesti, [palauttamalla käyttäjän Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="44ba2-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="44ba2-111">Huomautus: Jos OneDrive tai SharePointin hallinta keskus ei ole usean sellaisen käyttäjän käytettävissä, joilla on aiemmin ollut käyttö oikeus, kyseessä voi olla tilapäinen palvelu ongelma.</span><span class="sxs-lookup"><span data-stu-id="44ba2-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="44ba2-112">[Tarkista palvelun kunnon koonti näyttö](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="44ba2-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


