---
title: Käytön estämien viestien vianmääritys
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505376"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="4853d-102">Access Denied -viestien vianmääritys Sharepointissa/OneDrive-hallintakeskuksessa</span><span class="sxs-lookup"><span data-stu-id="4853d-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="4853d-103">Jos saat käyttöestetty -sanoman, kun yrität selata Sharepoint/OneDrive-hallintakeskusta, varmista, että [määrität käyttäjälle käyttöoikeuden.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="4853d-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="4853d-104">Jos käyttäjällä on käyttöoikeus, varmista myös, että [hänelle on määritetty järjestelmänvalvojan rooli,](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) joka voi käyttää hallintakeskuksia.</span><span class="sxs-lookup"><span data-stu-id="4853d-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="4853d-105">Tämä ongelma voi ilmetä myös silloin, kun käyttäjä poistetaan ja luodaan uudelleen samalla käyttäjänimellä (UPN).</span><span class="sxs-lookup"><span data-stu-id="4853d-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="4853d-106">Uusi tili luodaan käyttämällä toista PUID (Passport Unique ID) -arvoa.</span><span class="sxs-lookup"><span data-stu-id="4853d-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="4853d-107">Kun käyttäjä yrittää käyttää sivustokokoelmaa tai OneDrivea, käyttäjällä on virheellinen PUID-tunnus.</span><span class="sxs-lookup"><span data-stu-id="4853d-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="4853d-108">Toinen skenaario koskee hakemistosynkronointia Active Directory -organisaatioyksikön kanssa.</span><span class="sxs-lookup"><span data-stu-id="4853d-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="4853d-109">Jos käyttäjät ovat jo kirjautuneet SharePointiin ja siirtyvät sitten toiseen organisaatioyksikköön ja synkronoivat sharepointin uudelleen, he saattavat kohdata tämän ongelman.</span><span class="sxs-lookup"><span data-stu-id="4853d-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="4853d-110">Voit ratkaista tämän ongelman palauttamalla alkuperäisen UPN-numeron artikkelin ohjeiden mukaisesti, [jotka artikkelissa Palauta käyttäjä Microsoft 365:ssä](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="4853d-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="4853d-111">Huomautus: Jos OneDrive- tai SharePoint-hallintakeskus ei ole käytettävissä useille käyttäjille, joilla on aiemmin ollut käyttöoikeus, saattaa olla tilapäinen palveluongelma.</span><span class="sxs-lookup"><span data-stu-id="4853d-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="4853d-112">[Tarkista palvelun kunnon koontinäyttö](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="4853d-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


