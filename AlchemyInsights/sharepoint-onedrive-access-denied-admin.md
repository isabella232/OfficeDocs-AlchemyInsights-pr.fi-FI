---
title: Vianmääritys viestit on estetty
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760338"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="f9e68-102">Käyttö estetty viestit Admin Centerissä Sharepoint/OneDrive liittyviä ongelmia</span><span class="sxs-lookup"><span data-stu-id="f9e68-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="f9e68-103">Jos saat käyttö estetty-sanoman, kun he yrittävät selata Sharepoint-/ OneDrive-hallintakeskukseen, varmista, että et [Määritä käyttöoikeus käyttäjälle](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="f9e68-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="f9e68-104">Jos käyttäjällä on käyttöoikeus, sinun olisi myös Varmista, että [määritetty järjestelmänvalvoja-rooli](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , voivat käyttää admin-keskukset ovat.</span><span class="sxs-lookup"><span data-stu-id="f9e68-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="f9e68-105">Tämä ongelma voi ilmetä myös, kun käyttäjä poistetaan ja luodaan uudelleen sama käyttäjätunnus (UPN) kanssa.</span><span class="sxs-lookup"><span data-stu-id="f9e68-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="f9e68-106">Uusi tili on luotu käyttämällä eri PUID (yksilöllisen Passport-tunnus)-arvoa.</span><span class="sxs-lookup"><span data-stu-id="f9e68-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="f9e68-107">Kun käyttäjä yrittää käyttää sivustokokoelman tai niiden OneDrive, käyttäjällä on virheellinen PUID.</span><span class="sxs-lookup"><span data-stu-id="f9e68-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="f9e68-108">Toinen tilanne liittyy directory-synkronointia Active Directoryn organisaatioyksikössä (OU).</span><span class="sxs-lookup"><span data-stu-id="f9e68-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="f9e68-109">Jos käyttäjät ovat jo kirjautuneena SharePoint-ovat siirretään eri OU ja SharePointin kanssa resynced, he saattavat kohdata tämän ongelman.</span><span class="sxs-lookup"><span data-stu-id="f9e68-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="f9e68-110">Voit ratkaista tämän ongelman, Palauta alkuperäiset UPN kanssa artikkelin, [Palauta Office 365-käyttäjä](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="f9e68-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="f9e68-111">Huomautus: Jos OneDrive tai SharePoint-Admin center ei ole aikaisemmin olleet tekemisissä useiden käyttäjien käytettävissä, saattaa olla väliaikaista palvelua ongelma.</span><span class="sxs-lookup"><span data-stu-id="f9e68-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="f9e68-112">[Tarkista palvelun terveyden dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="f9e68-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


