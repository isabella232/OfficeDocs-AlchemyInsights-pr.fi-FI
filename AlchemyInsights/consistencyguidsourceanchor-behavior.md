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
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor-toiminta

Azure AD Connect (versio 1.1.524.0 ja uudempi) helpottaa nyt msDS-ConsistencyGuidin käyttöä sourceAnchor-määritteenä. Kun käytät tätä ominaisuutta, Azure AD Connect määrittää synkronointisäännöt automaattisesti
  
- Käytä msDS-ConsistencyGuid-määritettä user-objektien sourceAnchor-määritteenä. ObjectGUID-objekteja käytetään muissa objektityypeissä.
    
- Azure AD Connect kirjoittaa objektinguid-arvon takaisin msDS-ConsistencyGuid-määritteeseen paikalliselle Active Directorylle minkä tahansa paikallisen AD User -objektin msDS-ConsistencyGuid-määritteen perusteella. Kun msDS-ConsistencyGuid-määrite on täytetty, Azure AD Connect vie objektin Azure AD:lle.
    
 **Huomautus:** Kun paikallinen AD-objekti on tuotu Azure AD Connectiin (joka tuodaan AD-yhdistintilaan ja ennustetaan Metaverseen), et voi enää muuttaa sen lähdearvoa. Jos haluat määrittää lähdearvon paikalliseen AD-objektiin, määritä sen msDS-ConsistencyGuid-määrite ennen sen tuomista Azure AD Connectiin. 
  
Lisätietoja SourceAnchor- ja ConsistencyGuid-tavoista on seuraavissa tavassa: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

