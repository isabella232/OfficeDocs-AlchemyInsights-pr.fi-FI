---
title: Yhdenmukaisencyguid/sourceAnchor-toiminto
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756280"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="d6408-102">Yhdenmukaisencyguid/sourceAnchor-toiminto</span><span class="sxs-lookup"><span data-stu-id="d6408-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="d6408-103">Azure AD Connect (versio 1.1.524.0 ja sen jälkeen) helpottaa tuki-ja liikunta elin sairauksien sekä Yhdenmukaisenpääguid-määritteen käyttöä sourceAnchor-määritteenä.</span><span class="sxs-lookup"><span data-stu-id="d6408-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="d6408-104">Kun käytät tätä ominaisuutta, Azure AD Connect määrittää synkronointi säännöt automaattisesti:</span><span class="sxs-lookup"><span data-stu-id="d6408-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="d6408-105">Käytä käyttöturvallisuustiedotteen-Yhdenmukaisenguid-määritettä käyttäjä objektien sourceAnchor-määritteenä.</span><span class="sxs-lookup"><span data-stu-id="d6408-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="d6408-106">Objeciguid-kohdetta käytetään muissa objekti tyypeissä.</span><span class="sxs-lookup"><span data-stu-id="d6408-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="d6408-107">Kaikissa paikallisessa AD-käyttäjä objektissa, jonka käyttöturvallisuustiedote on ei täytetty, Azure AD Connect kirjoittaa sen Objekguid-arvon takaisin paikallisen Active Directoryn MSDS-Condencyguid-määritteeseen.</span><span class="sxs-lookup"><span data-stu-id="d6408-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="d6408-108">Kun käyttöturvallisuustiedotteen-Yhdenmukaisenguid-määrite on täytetty, Azure AD Connect vie objektin Azure AD:hen.</span><span class="sxs-lookup"><span data-stu-id="d6408-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="d6408-109">**Huomautus:** Kun paikallinen mainos objekti tuodaan Azure AD Connectiin (eli tuodaan mainoksen yhdistin-tilaan ja ennustetaan metaversumiin), et voi enää muuttaa sen sourceAnchor-arvoa.</span><span class="sxs-lookup"><span data-stu-id="d6408-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="d6408-110">Jos haluat määrittää sourceAnchor-arvon tiettyä paikallista mainos objektia varten, määritä sen MSDS-Condencyguid-määrite, ennen kuin se tuodaan Azure AD Connectiin.</span><span class="sxs-lookup"><span data-stu-id="d6408-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="d6408-111">Lisä tietoja SourceAnchor-ja Condencyguid-tunnuksista on seuraavissa artikkeleissa: [Azure AD Connect: suunnittelu käsitteet](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="d6408-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

