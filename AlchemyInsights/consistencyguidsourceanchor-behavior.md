---
title: ConsistencyGuid / sourceAnchor käyttäytyminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705730"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor käyttäytyminen

Azure AD Connect (versio 1.1.524.0 ja sen jälkeen) helpottaa nyt msDS-ConsistencyGuidin käyttöä sourceAnchor-määritteenä. Kun käytät tätä ominaisuutta, Azure AD Connect määrittää synkronointisäännöt automaattisesti seuraavasti:
  
- Käytä msDS-ConsistencyGuid-tunnusta useranchor-määritteenä käyttäjäobjekteille. ObjectGUID-kohdetta käytetään muissa objektityypeissä.
    
- Azure AD Connect kirjoittaa objektiGUID-arvonsa takaisin paikallisen Active Directoryn msDS-ConsistencyGuid-määritteeseen, jonka msDS-ConsistencyGuid-määritettä ei ole täytetty. Kun msDS-ConsistencyGuid-määrite on täytetty, Azure AD Connect vie objektin Azure AD:hen.
    
 **Huomautus:** Kun paikallinen AD-objekti on tuotu Azure AD Connectiin (eli tuotu AD Connector Spaceen ja heijastettu Metaverse-tilaan), et voi enää muuttaa sen sourceAnchor-arvoa. Jos haluat määrittää sourceAnchor-arvon tietylle paikalliselle AD-objektille, määritä sen msDS-ConsistencyGuid-määrite ennen sen tuomista Azure AD Connectiin. 
  
Lisätietoja SourceAnchorista ja ConsistencyGuidistä on seuraavissa ohjeaiheissa: [Azure AD Connect: Suunnittelukäsitteet](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

