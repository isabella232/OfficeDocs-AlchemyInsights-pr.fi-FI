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
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/15/2019
ms.locfileid: "36516975"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor-käyttäytyminen

Azure AD Connect (versio 1.1.524.0 ja sen jälkeen) helpottaa nyt msDS-ConsistencyGuid-määritteen käyttämistä sourceAnchor-määritteenä. Kun käytät tätä ominaisuutta, Azure AD Connect määrittää synkronointi säännöt automaattisesti:
  
- Käytä msDS-ConsistencyGuid: ää käyttäjä objektien sourceAnchor-määritteenä. ObjectGUID-tunnusta käytetään muissa objekti tyypeissä.
    
- Jos kyseessä on paikallinen mainos käyttäjä objekti, jonka msDS-ConsistencyGuid-määritettä ei ole täytetty, Azure AD Connect kirjoittaa objectGUID-arvonsa paikalliseen Active Directoryyn msDS-ConsistencyGuid-määritteeseen. Kun msDS-ConsistencyGuid-määrite on täytetty, Azure AD Connect vie objektin Azure AD:een.
    
 **Huom:** Kun paikallinen mainos objekti tuodaan Azure AD Connectin (joka tuodaan AD Connector-tilaan ja projisoidaan Metaverse-arvoksi), et voi enää muuttaa sen sourceAnchor-arvoa. Määritä tietyn paikallisen mainos objektin sourceAnchor-arvo määrittämällä sen msDS-ConsistencyGuid-määrite, ennen kuin se tuodaan Azure AD Connectin kautta. 
  
Lisä tietoja SourceAnchor-ja ConsistencyGuid-objekteistä on seuraavissa: [Azure AD Connect: suunnittelun käsitteet](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

