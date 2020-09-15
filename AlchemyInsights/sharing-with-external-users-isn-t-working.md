---
title: Jakaminen ulkopuolisten käyttäjien kanssa ei toimi
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691572"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="ca2f2-102">SharePoint-sisällön jakamiseen ulkoisiin käyttäjiin liittyvien ongelmien korjaaminen</span><span class="sxs-lookup"><span data-stu-id="ca2f2-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="ca2f2-103">Varmista, että ulkoinen jakaminen on otettu käyttöön organisaatiossa:</span><span class="sxs-lookup"><span data-stu-id="ca2f2-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="ca2f2-104">Siirry [ &amp; Microsoft 365-hallinta keskuksen palvelut-apuohjelmat-sivulle](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)ja valitse **sivustot**.</span><span class="sxs-lookup"><span data-stu-id="ca2f2-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="ca2f2-105">Varmista, että asetus on käytössä.</span><span class="sxs-lookup"><span data-stu-id="ca2f2-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="ca2f2-106">Jos vain olemassa olevat ulkoiset käyttäjät-kohta on valittuna, varmista, että ulkoinen käyttäjä on lueteltu Microsoft 365-hallinta keskuksessa.</span><span class="sxs-lookup"><span data-stu-id="ca2f2-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="ca2f2-107">Varmista, että ulkoinen jakaminen on otettu käyttöön sivustossa.</span><span class="sxs-lookup"><span data-stu-id="ca2f2-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="ca2f2-108">Perinteinen sivustokokoelma:</span><span class="sxs-lookup"><span data-stu-id="ca2f2-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="ca2f2-109">Valitse uusi SharePoint-hallinta keskus-kohdan vasemmanpuoleisessa ruudussa **sivustot**.</span><span class="sxs-lookup"><span data-stu-id="ca2f2-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="ca2f2-110">Valitse sivusto tai sivustot ja valitse sitten valinta nauhassa **jakaminen**.</span><span class="sxs-lookup"><span data-stu-id="ca2f2-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="ca2f2-111">Ryhmäsivusto, joka kuuluu Microsoft 365-ryhmään tai viestintäsivustoon:</span><span class="sxs-lookup"><span data-stu-id="ca2f2-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="ca2f2-112">Näillä uusilla sivustotyypeillä on sama jakamis asetus koko organisaation leveää asetusta varten, ellei koko organisaation laajuinen asetus salli tiedostojen jakamista linkeillä, jotka eivät edellytä sisäänkirjautumista.</span><span class="sxs-lookup"><span data-stu-id="ca2f2-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="ca2f2-113">Tässä tapa uksessa sivustot sallivat jakamisen uusilla ja olemassa oleville ulkoisille käyttäjille, jotka kirjautuvat sisään.</span><span class="sxs-lookup"><span data-stu-id="ca2f2-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="ca2f2-114">Jos haluat muuttaa tiettyjen sivuston asetuksia, käytä uutta SharePoint-hallinta keskusta tai PowerShelliä.</span><span class="sxs-lookup"><span data-stu-id="ca2f2-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="ca2f2-115">[Lisätietoja](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="ca2f2-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="ca2f2-116">Minkä tahansa sivuston ulkoinen jakamis asetus voi olla organisaatiolaajuista asetusta rajoittavampi, mutta ei koko organisaatiota leveää asetusta suurempi.</span><span class="sxs-lookup"><span data-stu-id="ca2f2-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

