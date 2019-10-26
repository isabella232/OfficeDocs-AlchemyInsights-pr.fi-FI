---
title: ConsistencyGuid/sourceAnchor-käyttäytyminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/25/2019
ms.locfileid: "36516975"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="b2427-102">ConsistencyGuid/sourceAnchor-käyttäytyminen</span><span class="sxs-lookup"><span data-stu-id="b2427-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="b2427-103">Azure AD Connect (versio 1.1.524.0 ja sen jälkeen) helpottaa nyt msDS-ConsistencyGuid-määritteen käyttämistä sourceAnchor-määritteenä.</span><span class="sxs-lookup"><span data-stu-id="b2427-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="b2427-104">Kun käytät tätä ominaisuutta, Azure AD Connect määrittää synkronointi säännöt automaattisesti:</span><span class="sxs-lookup"><span data-stu-id="b2427-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="b2427-105">Käytä msDS-ConsistencyGuid: ää käyttäjä objektien sourceAnchor-määritteenä.</span><span class="sxs-lookup"><span data-stu-id="b2427-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="b2427-106">ObjectGUID-tunnusta käytetään muissa objekti tyypeissä.</span><span class="sxs-lookup"><span data-stu-id="b2427-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="b2427-107">Jos kyseessä on paikallinen mainos käyttäjä objekti, jonka msDS-ConsistencyGuid-määritettä ei ole täytetty, Azure AD Connect kirjoittaa objectGUID-arvonsa paikalliseen Active Directoryyn msDS-ConsistencyGuid-määritteeseen.</span><span class="sxs-lookup"><span data-stu-id="b2427-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="b2427-108">Kun msDS-ConsistencyGuid-määrite on täytetty, Azure AD Connect vie objektin Azure AD:een.</span><span class="sxs-lookup"><span data-stu-id="b2427-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="b2427-109">**Huom:** Kun paikallinen mainos objekti tuodaan Azure AD Connectin (joka tuodaan AD Connector-tilaan ja projisoidaan Metaverse-arvoksi), et voi enää muuttaa sen sourceAnchor-arvoa.</span><span class="sxs-lookup"><span data-stu-id="b2427-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="b2427-110">Määritä tietyn paikallisen mainos objektin sourceAnchor-arvo määrittämällä sen msDS-ConsistencyGuid-määrite, ennen kuin se tuodaan Azure AD Connectin kautta.</span><span class="sxs-lookup"><span data-stu-id="b2427-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="b2427-111">Lisä tietoja SourceAnchor-ja ConsistencyGuid-objekteistä on seuraavissa: [Azure AD Connect: suunnittelun käsitteet](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="b2427-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

