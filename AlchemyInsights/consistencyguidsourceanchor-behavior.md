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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044337"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor-toiminta

Azure AD Näyttöyhteys (versio 1.1.524.0 ja uudempi) helpottaa nyt msDS-ConsistencyGuidin käyttöä sourceAnchor-määritteenä. Kun käytät tätä ominaisuutta, Azure AD Näyttöyhteys määrittää synkronointisäännöt automaattisesti
  
- Käytä msDS-ConsistencyGuid-määritettä user-objektien sourceAnchor-määritteenä. ObjectGUID-objekteja käytetään muissa objektityypeissä.
    
- Azure AD Näyttöyhteys kirjoittaa objektinGUID-arvon takaisin msDS-ConsistencyGuid-määritteeseen paikalliselle Active Directorylle minkä tahansa paikallisen AD User -objektin, jonka msDS-ConsistencyGuid-määritettä ei ole täytetty. Kun msDS-ConsistencyGuid-määrite on täytetty, Azure AD Näyttöyhteys vie objektin Azure AD:lle.
    
 **Huomautus:** Kun paikallinen AD-objekti on tuotu Azure AD Näyttöyhteys:een (joka tuodaan AD-yhdistintilaan ja ennustetaan Metaverse-objektiin), et voi enää muuttaa sen lähdearvoa. Jos haluat määrittää lähdearvon paikalliselle AD-objektille, määritä sen msDS-ConsistencyGuid-määrite, ennen kuin se tuodaan Azure AD Näyttöyhteys. 
  
Lisätietoja SourceAnchor- ja ConsistencyGuid-tavoista on seuraavassa: [Azure AD Näyttöyhteys: Suunnittelukäsitteet](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

