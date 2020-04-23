---
title: Jakaminen ulkoisten käyttäjien kanssa ei toimi
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 285535d6144825f0935bf72579a483260c2f2bd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767246"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="47bea-102">SharePoint-sisällön jakamiseen ulkoisten käyttäjien kanssa liittyvien ongelmien korjaaminen</span><span class="sxs-lookup"><span data-stu-id="47bea-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="47bea-103">Varmista, että ulkoinen jakaminen on käytössä organisaatiossasi:</span><span class="sxs-lookup"><span data-stu-id="47bea-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="47bea-104">Siirry [Microsoft &amp; 365 -hallintakeskuksen Palvelut-apuohjelmat -sivulle](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)ja valitse **Sivustot**.</span><span class="sxs-lookup"><span data-stu-id="47bea-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="47bea-105">Varmista, että asetuksen asetuksena on Käytössä.</span><span class="sxs-lookup"><span data-stu-id="47bea-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="47bea-106">Jos "Vain nykyiset ulkoiset käyttäjät" on valittuna, varmista, että ulkoinen käyttäjä näkyy Microsoft 365 -hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="47bea-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="47bea-107">Varmista, että ulkoinen jakaminen on käytössä sivustossa.</span><span class="sxs-lookup"><span data-stu-id="47bea-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="47bea-108">Klassista sivustokokoelmaa varten:</span><span class="sxs-lookup"><span data-stu-id="47bea-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="47bea-109">Valitse uuden SharePoint-hallintakeskuksen vasemmanpuoleisesta ruudusta **Sivustot**.</span><span class="sxs-lookup"><span data-stu-id="47bea-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="47bea-110">Valitse sivusto tai sivustot ja valitse valintanauhasta **Jakaminen**.</span><span class="sxs-lookup"><span data-stu-id="47bea-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="47bea-111">Ryhmäsivustossa, joka kuuluu Office 365 -ryhmään tai viestintäsivustoon:</span><span class="sxs-lookup"><span data-stu-id="47bea-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="47bea-112">Näillä uusilla sivustotyypeillä on sama jakamisasetus kuin organisaation laajuisella asetuksella, ellei organisaation laajuinen asetus salli tiedostojen jakamista linkeillä, jotka eivät edellytä kirjautumista.</span><span class="sxs-lookup"><span data-stu-id="47bea-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="47bea-113">Tässä tapauksessa sivustot sallivat jakamisen uusien ja olemassa olevien ulkoisten käyttäjien kanssa, jotka kirjautuvat sisään.</span><span class="sxs-lookup"><span data-stu-id="47bea-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="47bea-114">Jos haluat muuttaa tiettyjen sivustojen asetusta, käytä uutta SharePoint-hallintakeskusta tai PowerShelliä.</span><span class="sxs-lookup"><span data-stu-id="47bea-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="47bea-115">[Lisätietoja](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="47bea-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="47bea-116">Minkä tahansa sivuston ulkoinen jakamisasetus voi olla rajoittavampi kuin koko organisaation asetus, mutta ei sallivampi kuin organisaation laajuinen asetus.</span><span class="sxs-lookup"><span data-stu-id="47bea-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

