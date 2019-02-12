---
title: ConsistencyGuid / sourceAnchor-ongelma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: e1ffa9cf2b59570cb6ea3517efad7a55fd9489a8
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29927637"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor-ongelma

Azure AD Connect (versio 1.1.524.0 jälkeen) nyt helpottaa käyttöä, koska msDS-ConsistencyGuid sourceAnchor määrite. Kun käytät tätä ominaisuutta, Azure AD Yhdistä määrittää synkronoinnin säännöt:
  
- Käyttää käyttöturvallisuustiedotteen-ConsistencyGuid sourceAnchor määrite käyttäjäobjekteja. ObjectGUID käytetään muiden kohteiden tyypit.
    
- Annettu jollekin paikallisen AD-käyttäjä objekti, jonka käyttöturvallisuustiedotteen ConsistencyGuid määrite ei ole täytetty, Azure AD Yhdistä kirjoituksia objectGUID arvonsa takaisin paikalliseen Active Directoryyn käyttöturvallisuustiedotteen-ConsistencyGuid-määritettä. Käyttöturvallisuustiedotteen ConsistencyGuid määrite täytetään, kun Azure AD Yhdistä Vie objekti sitten Azure AD.
    
 **Huomautus:** Kerran paikallisen AD-objekti tuodaan Azure AD-muodosta (eli, tuodaan AD Connector-tilaa ja suunniteltu yhdeksi Metaverse), sen sourceAnchor-arvoa ei voi muuttaa enää. Määritä sourceAnchor arvo antanut paikallisen AD määrittää sen koska ConsistencyGuid määritteen, ennen kuin se tuodaan Azure AD Connect-objektia. 
  
Lisätietoja SourceAnchor ja ConsistencyGuid viittaavat seuraavasti: [Azure AD Yhdistä: käsitteet suunnitella](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

