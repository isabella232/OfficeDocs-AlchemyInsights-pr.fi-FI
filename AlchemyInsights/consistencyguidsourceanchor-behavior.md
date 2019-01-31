---
title: ConsistencyGuid / sourceAnchor-ongelma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 010474bcc4cc6f97bcaafef9dfe6f4accfed4247
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/30/2019
ms.locfileid: "29659588"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor-ongelma

Azure AD Connect (versio 1.1.524.0 jälkeen) nyt helpottaa käyttöä, koska msDS-ConsistencyGuid sourceAnchor määrite. Kun käytät tätä ominaisuutta, Azure AD Yhdistä määrittää synkronoinnin säännöt:
  
- Käyttää käyttöturvallisuustiedotteen-ConsistencyGuid sourceAnchor määrite käyttäjäobjekteja. ObjectGUID käytetään muiden kohteiden tyypit.
    
- Annettu jollekin paikallisen AD-käyttäjä objekti, jonka käyttöturvallisuustiedotteen ConsistencyGuid määrite ei ole täytetty, Azure AD Yhdistä kirjoituksia objectGUID arvonsa takaisin paikalliseen Active Directoryyn käyttöturvallisuustiedotteen-ConsistencyGuid-määritettä. Käyttöturvallisuustiedotteen ConsistencyGuid määrite täytetään, kun Azure AD Yhdistä Vie objekti sitten Azure AD.
    
 **Huomautus:** Kerran paikallisen AD-objekti tuodaan Azure AD-muodosta (eli, tuodaan AD Connector-tilaa ja suunniteltu yhdeksi Metaverse), sen sourceAnchor-arvoa ei voi muuttaa enää. Määritä sourceAnchor arvo antanut paikallisen AD määrittää sen koska ConsistencyGuid määritteen, ennen kuin se tuodaan Azure AD Connect-objektia. 
  
Lisätietoja SourceAnchor ja ConsistencyGuid viittaavat seuraavasti: [Azure AD Yhdistä: käsitteet suunnitella](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

