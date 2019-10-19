---
title: Jakaminen ulkoisten käyttäjien kanssa ei toimi
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502228"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="5f5c0-102">SharePoint-sisältöä ulkoisten käyttäjien kanssa jakavan ongelman korjaaminen</span><span class="sxs-lookup"><span data-stu-id="5f5c0-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="5f5c0-103">Varmista, että ulkoinen jakaminen on käytössä organisaatiossa:</span><span class="sxs-lookup"><span data-stu-id="5f5c0-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="5f5c0-104">Siirry [ &amp; Palvelut-apuohjelmat-sivulle Microsoft 365-hallinta keskuksessa](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)ja valitse **sivustot**.</span><span class="sxs-lookup"><span data-stu-id="5f5c0-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="5f5c0-105">Varmista, että asetus on käytössä.</span><span class="sxs-lookup"><span data-stu-id="5f5c0-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="5f5c0-106">Jos valittuna on "vain nykyiset ulkoiset käyttäjät", varmista, että ulkoinen käyttäjä näkyy Microsoft 365-hallinta keskuksessa.</span><span class="sxs-lookup"><span data-stu-id="5f5c0-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="5f5c0-107">Varmista, että ulkoinen jakaminen on käytössä sivustolla.</span><span class="sxs-lookup"><span data-stu-id="5f5c0-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="5f5c0-108">Klassiseen sivustokokoelmaan:</span><span class="sxs-lookup"><span data-stu-id="5f5c0-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="5f5c0-109">Valitse uudessa SharePointin hallinta keskuksessa vasemmassa ruudussa **sivustot**.</span><span class="sxs-lookup"><span data-stu-id="5f5c0-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="5f5c0-110">Valitse sivusto tai sivustot ja valitse sitten valinta nauhassa **jakaminen**.</span><span class="sxs-lookup"><span data-stu-id="5f5c0-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="5f5c0-111">Office 365-ryhmään kuuluva ryhmäsivusto tai tieto liikenne sivusto:</span><span class="sxs-lookup"><span data-stu-id="5f5c0-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="5f5c0-112">Näillä uusilla sivustotyypeilla on sama jakamis asetus kuin organisaatiolla-asetuksella, ellei organisaation laajuinen asetus sallii tiedostojen jakamista sellaisten linkkien avulla, jotka eivät vaadi kirjautumista.</span><span class="sxs-lookup"><span data-stu-id="5f5c0-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="5f5c0-113">Tässä tapa uksessa sivustot sallivat jakamisen uusille ja olemassa oleville ulkoisille käyttäjille, jotka kirjautumiseen.</span><span class="sxs-lookup"><span data-stu-id="5f5c0-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="5f5c0-114">Jos haluat muuttaa tiettyjen sivustojen asetuksia, käytä uutta SharePointin hallinta keskusta tai PowerShelliä.</span><span class="sxs-lookup"><span data-stu-id="5f5c0-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="5f5c0-115">[Lue lisää](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="5f5c0-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="5f5c0-116">Ulkoisen jakamisen asetus missä tahansa sivustossa voi olla rajoittavampi kuin koko organisaatiota koskeva asetus, mutta ei enemmän salliva kuin organisaation laajuinen asetus.</span><span class="sxs-lookup"><span data-stu-id="5f5c0-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

