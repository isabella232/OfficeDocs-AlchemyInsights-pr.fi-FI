---
title: Estettyjen viestien käytön vianmääritys
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759797"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="188eb-102">Estettyjen viestien käytön vianmääritys</span><span class="sxs-lookup"><span data-stu-id="188eb-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="188eb-103">Jos joku sai Käyttö estetty -sanoman SharePointin jaettuun kansioon, sivustokokoelman järjestelmänvalvoja on saattanut ottaa käyttöön rajoitetun käytön käyttöoikeudet -lukitustilan.</span><span class="sxs-lookup"><span data-stu-id="188eb-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="188eb-104">Voit poistaa tämän käytöstä:</span><span class="sxs-lookup"><span data-stu-id="188eb-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="188eb-105">Selaa sivustoon, napsauta Asetukset-kuvaketta ja valitse sitten **Sivuston asetukset**.</span><span class="sxs-lookup"><span data-stu-id="188eb-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="188eb-106">Valitse **Sivustokokoelman hallinta**-kohdasta **Sivustokokoelman ominaisuudet**.</span><span class="sxs-lookup"><span data-stu-id="188eb-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="188eb-107">Valitse **Rajoitetun käytön käyttöoikeudet -kohdan**vierestä **Poista aktivointi**.</span><span class="sxs-lookup"><span data-stu-id="188eb-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="188eb-108">Käyttö estetty -sanoma voi ilmetä myös jaetuissa kansioissa, jos sivusto on julkaisusivusto.</span><span class="sxs-lookup"><span data-stu-id="188eb-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="188eb-109">Lisätietoja on [ohjeaiheessa Käyttö estetty jaetun kansion käytön yhteydessä](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="188eb-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="188eb-110">Jos joku sai Käyttö estetty -sanoman yrittäessään tarkastella käyttöoikeuspyyntöjä, käyttäjä on lisättävä joko sivustokokoelman järjestelmänvalvojana tai sivuston Omistajat-ryhmän jäsenenä.</span><span class="sxs-lookup"><span data-stu-id="188eb-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="188eb-111">Lisätietoja on [ohjeaiheessa Käyttö estetty -luettelo](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="188eb-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="188eb-112">Jos käyttäjä sai Käyttö estetty -sanoman sen jälkeen, kun hänet on poistettu paikallisesta Active Directorysta ja lisätty sitten takaisin, katso [lisätietoja ohjeaiheesta Käyttö estetty, kun käyttäjätili synkronoidaan Microsoft 365:een](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="188eb-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

