---
title: Ulkoisten käyttäjien kanssa ei toimi
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
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747595"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="0bbca-102">SharePoint-sisällön jakaminen ulkoisten käyttäjien ongelmien korjaaminen</span><span class="sxs-lookup"><span data-stu-id="0bbca-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="0bbca-103">Varmista, että ulkoinen jakaminen on otettu käyttöön organisaatiossa:</span><span class="sxs-lookup"><span data-stu-id="0bbca-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="0bbca-104">Siirry [palvelut &amp; apuohjelmia Microsoft 365 admin keskellä sivun](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), ja valitse **sivustot**.</span><span class="sxs-lookup"><span data-stu-id="0bbca-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="0bbca-105">Varmista, että asetus on poistettu ”käytössä”.</span><span class="sxs-lookup"><span data-stu-id="0bbca-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="0bbca-106">Jos ”vain olemassa olevat Ulkoiset käyttäjät” on valittuna, varmista, että ulkoisen käyttäjän tiedot on lueteltu Microsoft 365 admin Centerissä.</span><span class="sxs-lookup"><span data-stu-id="0bbca-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="0bbca-107">Varmista, että ulkoinen jakamisen pois sivuston.</span><span class="sxs-lookup"><span data-stu-id="0bbca-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="0bbca-108">Perinteinen sivustokokoelman:</span><span class="sxs-lookup"><span data-stu-id="0bbca-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="0bbca-109">Valitse uuden SharePoint-hallintakeskukseen vasemmanpuoleisessa ruudussa **sivustot**.</span><span class="sxs-lookup"><span data-stu-id="0bbca-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="0bbca-110">Valitse sivusto tai sivustoja ja valitse valintanauhan **jakaminen**.</span><span class="sxs-lookup"><span data-stu-id="0bbca-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="0bbca-111">Ryhmäsivusto, joka kuuluu Office 365-ryhmään tai Viestimissivusto:</span><span class="sxs-lookup"><span data-stu-id="0bbca-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="0bbca-112">Tällaisten sivusto on sama jakamisen määrittäminen organisaation laajuisten asetusten paitsi koko organisaation-asetuksen avulla, jakaa tiedostoja, linkkejä, jotka eivät edellytä sisään.</span><span class="sxs-lookup"><span data-stu-id="0bbca-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="0bbca-113">Tässä tapauksessa sivustot sallivat uusien ja olemassa olevien ulkoisten käyttäjille, jotka kirjautua sisään jakaminen.</span><span class="sxs-lookup"><span data-stu-id="0bbca-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="0bbca-114">Voit muuttaa asetusta tietyissä sivustoissa, käyttämällä uutta SharePoint-hallintakeskukseen tai PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0bbca-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="0bbca-115">[Lue lisää](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="0bbca-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="0bbca-116">Kaikki sivuston ulkoinen jakaminen asetus voi olla rajoittavampi kuin organisaation laajuinen asetus, mutta ei kuitenkaan enempää kuin organisaation laajuinen asetus sallivien.</span><span class="sxs-lookup"><span data-stu-id="0bbca-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

