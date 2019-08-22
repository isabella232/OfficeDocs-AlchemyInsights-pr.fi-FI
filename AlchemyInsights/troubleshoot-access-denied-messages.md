---
title: Vianmääritys viestit on estetty
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: e4fea7188bd77ba876e2a245414372c3ff836059
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500399"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="e39de-102">Vianmääritys viestit on estetty</span><span class="sxs-lookup"><span data-stu-id="e39de-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="e39de-103">Jos joku sai ”käyttö estetty”-virhesanoman jaetun kansion SharePoint-sivustokokoelman järjestelmänvalvoja ehkä ottanut ”käyttöoikeus on rajoitettu käyttäjän oikeudet lockdown tilassa”.</span><span class="sxs-lookup"><span data-stu-id="e39de-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="e39de-104">Jos haluat poistaa käytöstä:</span><span class="sxs-lookup"><span data-stu-id="e39de-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="e39de-105">Siirry sivustoon asetukset-kuvaketta ja valitse sitten **Sivuston asetukset**.</span><span class="sxs-lookup"><span data-stu-id="e39de-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="e39de-106">Valitse **Sivustokokoelman hallinta**-kohdasta **sivustokokoelmaominaisuudet**.</span><span class="sxs-lookup"><span data-stu-id="e39de-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="e39de-107">Vieressä **käyttöoikeus on rajoitettu käyttöoikeus lockdown tilassa**Valitse **Poista aktivointi**.</span><span class="sxs-lookup"><span data-stu-id="e39de-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="e39de-108">Käyttö estetty-virhesanoman voi myös ilmetä jaettuja kansioita, jos sivusto on sivuston julkaiseminen.</span><span class="sxs-lookup"><span data-stu-id="e39de-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="e39de-109">Info Katso [Käyttö estetty muodostaessaan yhteyden jaettuun kansioon](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="e39de-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="e39de-110">Jos joku sai ”käyttö estetty”-virhesanoman yritettäessä tarkastella käyttöpyyntöjä, käyttäjän täytyy lisätä joko sivustokokoelman järjestelmänvalvoja tai sivuston omistajat-ryhmän jäsenenä.</span><span class="sxs-lookup"><span data-stu-id="e39de-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="e39de-111">Lisätietoja Katso [Käyttöoikeuspyyntöjä luetteloon on estetty](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="e39de-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="e39de-112">Jos käyttäjä sai ”käyttö estetty”-virhesanoman, kun he olivat Active Directoryn tiloista poistetaan ja lisätään sitten takaisin, katso [Käyttö estetty kun käyttäjätili on synkronoitu Office 365: ssä](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="e39de-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

