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
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516975"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor-ongelma

Azure AD Connect (versio 1.1.524.0 jälkeen) nyt helpottaa käyttöä, koska msDS-ConsistencyGuid sourceAnchor määrite. Kun käytät tätä ominaisuutta, Azure AD Yhdistä määrittää synkronoinnin säännöt:
  
- Käyttää käyttöturvallisuustiedotteen-ConsistencyGuid sourceAnchor määrite käyttäjäobjekteja. ObjectGUID käytetään muiden kohteiden tyypit.
    
- Annettu jollekin paikallisen AD-käyttäjä objekti, jonka käyttöturvallisuustiedotteen ConsistencyGuid määrite ei ole täytetty, Azure AD Yhdistä kirjoituksia objectGUID arvonsa takaisin paikalliseen Active Directoryyn käyttöturvallisuustiedotteen-ConsistencyGuid-määritettä. Käyttöturvallisuustiedotteen ConsistencyGuid määrite täytetään, kun Azure AD Yhdistä Vie objekti sitten Azure AD.
    
 **Huomautus:** Kerran paikallisen AD-objekti tuodaan Azure AD-muodosta (eli, tuodaan AD Connector-tilaa ja suunniteltu yhdeksi Metaverse), sen sourceAnchor-arvoa ei voi muuttaa enää. Määritä sourceAnchor arvo antanut paikallisen AD määrittää sen koska ConsistencyGuid määritteen, ennen kuin se tuodaan Azure AD Connect-objektia. 
  
Lisätietoja SourceAnchor ja ConsistencyGuid viittaavat seuraavasti: [Azure AD Yhdistä: käsitteet suunnitella](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

