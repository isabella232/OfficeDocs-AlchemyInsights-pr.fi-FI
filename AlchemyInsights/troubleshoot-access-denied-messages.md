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
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704891"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="7bb86-102">Käyttö estettyjen viestien vianmääritys</span><span class="sxs-lookup"><span data-stu-id="7bb86-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="7bb86-103">Jos joku sai Käyttö estetty -viestin jaettuun kansioon SharePointissa, sivustokokoelman järjestelmänvalvoja on saattanut ottaa käyttöön rajoitetun käytön käyttöoikeuksien lukittumistilan.</span><span class="sxs-lookup"><span data-stu-id="7bb86-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="7bb86-104">Voit poistaa tämän käytöstä näin:</span><span class="sxs-lookup"><span data-stu-id="7bb86-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="7bb86-105">Siirry sivustoon, napsauta Asetukset-kuvaketta ja valitse sitten **Sivuston asetukset.**</span><span class="sxs-lookup"><span data-stu-id="7bb86-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="7bb86-106">Valitse **Sivustokokoelman hallinta**-kohdassa **Sivustokokoelman ominaisuudet.**</span><span class="sxs-lookup"><span data-stu-id="7bb86-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="7bb86-107">Valitse **Rajoitetun käyttöoikeuden lukittu tila -kohdan vierestä** Poista **aktivointi.**</span><span class="sxs-lookup"><span data-stu-id="7bb86-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="7bb86-108">Käyttö estetty -sanoma voi ilmetä myös jaetuissa kansioissa, jos sivusto on julkaisusivusto.</span><span class="sxs-lookup"><span data-stu-id="7bb86-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="7bb86-109">Lisätietoja on ohjeaiheessa Käyttö estetty [käytettäessä jaettua kansiota.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)</span><span class="sxs-lookup"><span data-stu-id="7bb86-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="7bb86-110">Jos käyttäjä sai Käyttö estetty -viestin, kun hän yrittää tarkastella käyttöoikeuspyyntöjä, käyttäjä on lisättävä joko sivustokokoelman järjestelmänvalvojaksi tai sivuston Omistajat-ryhmän jäsen.</span><span class="sxs-lookup"><span data-stu-id="7bb86-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="7bb86-111">Lisätietoja on kohdassa Käyttö estetty [pyyntöjen luettelossa.](https://go.microsoft.com/fwlink/?linkid=2004220)</span><span class="sxs-lookup"><span data-stu-id="7bb86-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="7bb86-112">Jos käyttäjä sai Käyttö estetty -viestin sen jälkeen, kun hänet on poistettu paikallisesta Active Directorysta ja lisätty takaisin, katso kohta Käyttö estetty, kun käyttäjätili on synkronoitu [Microsoft 365:lle.](https://go.microsoft.com/fwlink/?linkid=2004318)</span><span class="sxs-lookup"><span data-stu-id="7bb86-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

