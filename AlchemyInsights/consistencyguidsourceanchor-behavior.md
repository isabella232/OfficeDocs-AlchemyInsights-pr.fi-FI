---
title: ConsistencyGuid/sourceAnchor-toiminta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816989"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="7d87b-102">ConsistencyGuid/sourceAnchor-toiminta</span><span class="sxs-lookup"><span data-stu-id="7d87b-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="7d87b-103">Azure AD Connect (versio 1.1.524.0 ja uudempi) helpottaa nyt msDS-ConsistencyGuidin käyttöä sourceAnchor-määritteenä.</span><span class="sxs-lookup"><span data-stu-id="7d87b-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="7d87b-104">Kun käytät tätä ominaisuutta, Azure AD Connect määrittää synkronointisäännöt automaattisesti</span><span class="sxs-lookup"><span data-stu-id="7d87b-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="7d87b-105">Käytä msDS-ConsistencyGuid-määritettä user-objektien sourceAnchor-määritteenä.</span><span class="sxs-lookup"><span data-stu-id="7d87b-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="7d87b-106">ObjectGUID-objekteja käytetään muissa objektityypeissä.</span><span class="sxs-lookup"><span data-stu-id="7d87b-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="7d87b-107">Azure AD Connect kirjoittaa objektinguid-arvon takaisin msDS-ConsistencyGuid-määritteeseen paikalliselle Active Directorylle minkä tahansa paikallisen AD User -objektin msDS-ConsistencyGuid-määritteen perusteella.</span><span class="sxs-lookup"><span data-stu-id="7d87b-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="7d87b-108">Kun msDS-ConsistencyGuid-määrite on täytetty, Azure AD Connect vie objektin Azure AD:lle.</span><span class="sxs-lookup"><span data-stu-id="7d87b-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="7d87b-109">**Huomautus:** Kun paikallinen AD-objekti on tuotu Azure AD Connectiin (joka tuodaan AD-yhdistintilaan ja ennustetaan Metaverseen), et voi enää muuttaa sen lähdearvoa.</span><span class="sxs-lookup"><span data-stu-id="7d87b-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="7d87b-110">Jos haluat määrittää lähdearvon paikalliseen AD-objektiin, määritä sen msDS-ConsistencyGuid-määrite ennen sen tuomista Azure AD Connectiin.</span><span class="sxs-lookup"><span data-stu-id="7d87b-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="7d87b-111">Lisätietoja SourceAnchor- ja ConsistencyGuid-tavoista on seuraavissa tavassa: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="7d87b-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

