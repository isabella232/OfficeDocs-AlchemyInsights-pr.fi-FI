---
title: Ulkoisten käyttäjien kanssa ei toimi
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 305b3891e6c83e27b5c55c13757640e6e9d51a81
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29467542"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="8ee19-102">SharePoint-sisällön jakaminen ulkoisten käyttäjien ongelmien korjaaminen</span><span class="sxs-lookup"><span data-stu-id="8ee19-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="8ee19-103">Varmista, että ulkoinen jakaminen on otettu käyttöön organisaatiossa:</span><span class="sxs-lookup"><span data-stu-id="8ee19-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="8ee19-104">Siirry [palvelut &amp; -apuohjelmat Office 365: n hallinnan keskellä sivun](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), ja valitse **sivustot**.</span><span class="sxs-lookup"><span data-stu-id="8ee19-104">Go to the [Services &amp; add-ins page in the Office 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="8ee19-p101">Varmista, että asetus on poistettu ”käytössä”. Jos ”vain olemassa olevat Ulkoiset käyttäjät” on valittuna, varmista, että ulkoinen käyttäjä on mainittu Office 365-hallintakeskukseen.</span><span class="sxs-lookup"><span data-stu-id="8ee19-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Office 365 admin center.</span></span>
    
<span data-ttu-id="8ee19-p102">Varmista, että ulkoinen jakamisen pois sivuston. Perinteinen sivustokokoelman:</span><span class="sxs-lookup"><span data-stu-id="8ee19-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="8ee19-109">Valitse **sivustokokoelmat**classic SharePoint-hallintakeskukseen vasemmanpuoleisessa ruudussa.</span><span class="sxs-lookup"><span data-stu-id="8ee19-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="8ee19-110">Valitse sivusto tai sivustoja ja valitse valintanauhan **jakaminen**.</span><span class="sxs-lookup"><span data-stu-id="8ee19-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="8ee19-111">Ryhmäsivusto, joka kuuluu Office 365-ryhmään tai Viestimissivusto:</span><span class="sxs-lookup"><span data-stu-id="8ee19-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="8ee19-p103">Tällaisten sivusto on sama jakamisen määrittäminen organisaation laajuisten asetusten paitsi koko organisaation-asetuksen avulla, jakaa tiedostoja, linkkejä, jotka eivät edellytä sisään. Tässä tapauksessa sivustot sallivat uusien ja olemassa olevien ulkoisten käyttäjille, jotka kirjautua sisään jakaminen. Voit muuttaa asetusta tietyissä sivustoissa, käyttämällä uuden SharePoint-hallintakeskukseen (esikatselu)- tai PowerShell. [Lue lisää](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="8ee19-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="8ee19-116">Kaikki sivuston ulkoinen jakaminen asetus voi olla rajoittavampi kuin organisaation laajuinen asetus, mutta ei kuitenkaan enempää kuin organisaation laajuinen asetus sallivien.</span><span class="sxs-lookup"><span data-stu-id="8ee19-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

