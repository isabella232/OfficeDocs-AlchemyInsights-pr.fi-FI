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
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690780"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="df3f5-102">Käyttö estetty-viestien vian määritys</span><span class="sxs-lookup"><span data-stu-id="df3f5-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="df3f5-103">Jos joku on saanut käyttö estetty-viestin jaettuun kansioon SharePointissa, sivustokokoelman järjestelmänvalvoja on ehkä ottanut käyttöön rajoitetun käytön käyttö oikeuksien lukitus tilan.</span><span class="sxs-lookup"><span data-stu-id="df3f5-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="df3f5-104">Poista tämä toiminto käytöstä seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="df3f5-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="df3f5-105">Siirry sivustoon, napsauta Asetukset-kuvaketta ja valitse sitten **sivuston asetukset**.</span><span class="sxs-lookup"><span data-stu-id="df3f5-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="df3f5-106">Valitse sivustokokoelman **hallinta**-kohdassa **sivustokokoelman ominaisuudet**.</span><span class="sxs-lookup"><span data-stu-id="df3f5-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="df3f5-107">Valitse **rajoitetun käytön käyttö oikeuksien lukitus tila**-kohdan vierestä **Poista Akti vointi**.</span><span class="sxs-lookup"><span data-stu-id="df3f5-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="df3f5-108">Käyttö estetty-viesti voi ilmetä myös jaetuissa kansioissa, jos sivusto on Julkaisusivusto.</span><span class="sxs-lookup"><span data-stu-id="df3f5-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="df3f5-109">Lisä tietoja on Ohje aiheessa [käyttö estetty, kun käytät jaettuun kansioon](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="df3f5-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="df3f5-110">Jos joku on saanut käyttö estetty-viestin, kun hän yrittää tarkastella käyttö oikeus pyyntöjä, käyttäjän on lisättävä sivusto sivustokokoelman järjestelmänvalvojaksi tai sivuston omistajat-ryhmän jäseneksi.</span><span class="sxs-lookup"><span data-stu-id="df3f5-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="df3f5-111">Lisä tietoja on Ohje aiheessa käyttö [estetty-pyyntöjen luettelossa](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="df3f5-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="df3f5-112">Jos käyttäjä on saanut käyttö estetty-viestin, kun hänet on poistettu paikallisesta Active Directorysta ja sitten lisätty takaisin, Katso lisä tietoja artikkelista [käyttö estetty, kun käyttäjä tili synkronoidaan Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="df3f5-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

