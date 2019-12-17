---
title: Käyttö estetty-sanomien vian määritys
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 05d12aee49b449e8a29e84021b41298fb9983859
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050702"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="63338-102">Käyttö estetty-sanomien vian määritys</span><span class="sxs-lookup"><span data-stu-id="63338-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="63338-103">Jos joku on saanut käyttö estetty-sanoman SharePointissa jaettuun kansioon, sivustokokoelman järjestelmänvalvoja on saattanut ottaa käyttöön rajoitetun käyttö oikeuden lukitus tilan.</span><span class="sxs-lookup"><span data-stu-id="63338-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="63338-104">Voit poistaa tämän käytöstä:</span><span class="sxs-lookup"><span data-stu-id="63338-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="63338-105">Siirry sivustoon, napsauta Asetukset-kuvaketta ja valitse **sivuston asetukset**.</span><span class="sxs-lookup"><span data-stu-id="63338-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="63338-106">Valitse sivustokokoelman **hallinta**-kohdasta **sivustokokoelmaan liittyvät ominaisuudet**.</span><span class="sxs-lookup"><span data-stu-id="63338-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="63338-107">Valitse **rajoitetun käyttö oikeuden lukitus tilan**vieressä **Poista Akti vointi**.</span><span class="sxs-lookup"><span data-stu-id="63338-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="63338-108">Jaetut kansiot voivat myös aiheuttaa käyttö estetty-sanoman, jos sivusto on Julkaisusivusto.</span><span class="sxs-lookup"><span data-stu-id="63338-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="63338-109">Lisä tietoja on kohdassa [käyttö estetty jaettua kansiota](https://go.microsoft.com/fwlink/?linkid=2004317)käytettäessä.</span><span class="sxs-lookup"><span data-stu-id="63338-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="63338-110">Jos käyttäjällä on käyttö estetty-sanoma yritettäessä tarkastella käyttö oikeus pyyntöjä, käyttäjä täytyy lisätä joko sivustokokoelman järjestelmänvalvojaksi tai sivuston omistajien ryhmän jäseneksi.</span><span class="sxs-lookup"><span data-stu-id="63338-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="63338-111">Lisä tietoja on kohdassa Access- [pyyntöjen luettelon käyttö estetty](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="63338-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="63338-112">Jos käyttäjä on saanut käyttö estetty-sanoman sen jälkeen, kun hänet on poistettu Active Directorysta paikallisesti ja lisätty takaisin, katso [käyttö estetty, kun käyttäjä tili synkronoidaan Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="63338-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

