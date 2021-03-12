---
title: Käyttö estettyjen viestien vianmääritys
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707951"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="673ea-102">Käyttö estettyjen viestien vianmääritys SharePoint- tai OneDrive-hallintakeskuksessa</span><span class="sxs-lookup"><span data-stu-id="673ea-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="673ea-103">Jos näyttöön tulee käyttö estetty -sanoma, kun yrität selata SharePoint- tai OneDrive-hallintakeskukseen, varmista, että määrität [käyttäjälle käyttöoikeuden.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="673ea-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="673ea-104">Jos käyttäjällä on käyttöoikeus, varmista myös, [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) että käyttäjälle on määritetty järjestelmänvalvojan rooli, joka voi käyttää hallintakeskuksia.</span><span class="sxs-lookup"><span data-stu-id="673ea-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="673ea-105">Tämä ongelma voi ilmetä myös silloin, kun käyttäjä poistetaan ja luodaan uudelleen samalla käyttäjätunnuksilla (UPN).</span><span class="sxs-lookup"><span data-stu-id="673ea-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="673ea-106">Uusi tili luodaan käyttämällä eri PUID (Passport Unique ID) -arvoa.</span><span class="sxs-lookup"><span data-stu-id="673ea-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="673ea-107">Kun käyttäjä yrittää käyttää sivustokokoelmaa tai OneDrivea, käyttäjällä on virheellinen PUID.</span><span class="sxs-lookup"><span data-stu-id="673ea-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="673ea-108">Toinen skenaario koskee hakemistosynkronointia Active Directory -organisaatioyksikön (OU) kanssa.</span><span class="sxs-lookup"><span data-stu-id="673ea-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="673ea-109">Jos käyttäjät ovat jo kirjautuneet SharePointiin ja heidät siirretään toiseen ou:han ja synkronoidaan uudelleen SharePointin kanssa, he saattavat kokea tämän ongelman.</span><span class="sxs-lookup"><span data-stu-id="673ea-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="673ea-110">Voit ratkaista tämän ongelman palauttaen alkuperäisen käyttäjätunnuksen artikkelin Palauta käyttäjä [Microsoft 365:ssä ohjeiden mukaisesti.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="673ea-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="673ea-111">Huomautus: Jos OneDrive- tai SharePoint-hallintakeskus ei ole käytettävissä useille käyttäjille, joilla oli aiemmin käyttöoikeus, voi olla tilapäinen palveluongelma.</span><span class="sxs-lookup"><span data-stu-id="673ea-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="673ea-112">[Tarkista palvelun kunto -koontinäyttö.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="673ea-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


