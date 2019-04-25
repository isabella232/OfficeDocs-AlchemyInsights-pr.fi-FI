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
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408105"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor-ongelma

Azure AD Connect (versio 1.1.524.0 jälkeen) nyt helpottaa käyttöä, koska msDS-ConsistencyGuid sourceAnchor määrite. Kun käytät tätä ominaisuutta, Azure AD Yhdistä määrittää synkronoinnin säännöt:
  
- Käyttää käyttöturvallisuustiedotteen-ConsistencyGuid sourceAnchor määrite käyttäjäobjekteja. ObjectGUID käytetään muiden kohteiden tyypit.
    
- Annettu jollekin paikallisen AD-käyttäjä objekti, jonka käyttöturvallisuustiedotteen ConsistencyGuid määrite ei ole täytetty, Azure AD Yhdistä kirjoituksia objectGUID arvonsa takaisin paikalliseen Active Directoryyn käyttöturvallisuustiedotteen-ConsistencyGuid-määritettä. Käyttöturvallisuustiedotteen ConsistencyGuid määrite täytetään, kun Azure AD Yhdistä Vie objekti sitten Azure AD.
    
 **Huomautus:** Kerran paikallisen AD-objekti tuodaan Azure AD-muodosta (eli, tuodaan AD Connector-tilaa ja suunniteltu yhdeksi Metaverse), sen sourceAnchor-arvoa ei voi muuttaa enää. Määritä sourceAnchor arvo antanut paikallisen AD määrittää sen koska ConsistencyGuid määritteen, ennen kuin se tuodaan Azure AD Connect-objektia. 
  
Lisätietoja SourceAnchor ja ConsistencyGuid viittaavat seuraavasti: [Azure AD Yhdistä: käsitteet suunnitella](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

