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
# <a name="consistencyguid--sourceanchor-behavior"></a>Yhdenmukaisencyguid/sourceAnchor-toiminto

Azure AD Connect (versio 1.1.524.0 ja sen jälkeen) helpottaa tuki-ja liikunta elin sairauksien sekä Yhdenmukaisenpääguid-määritteen käyttöä sourceAnchor-määritteenä. Kun käytät tätä ominaisuutta, Azure AD Connect määrittää synkronointi säännöt automaattisesti:
  
- Käytä käyttöturvallisuustiedotteen-Yhdenmukaisenguid-määritettä käyttäjä objektien sourceAnchor-määritteenä. Objeciguid-kohdetta käytetään muissa objekti tyypeissä.
    
- Kaikissa paikallisessa AD-käyttäjä objektissa, jonka käyttöturvallisuustiedote on ei täytetty, Azure AD Connect kirjoittaa sen Objekguid-arvon takaisin paikallisen Active Directoryn MSDS-Condencyguid-määritteeseen. Kun käyttöturvallisuustiedotteen-Yhdenmukaisenguid-määrite on täytetty, Azure AD Connect vie objektin Azure AD:hen.
    
 **Huomautus:** Kun paikallinen mainos objekti tuodaan Azure AD Connectiin (eli tuodaan mainoksen yhdistin-tilaan ja ennustetaan metaversumiin), et voi enää muuttaa sen sourceAnchor-arvoa. Jos haluat määrittää sourceAnchor-arvon tiettyä paikallista mainos objektia varten, määritä sen MSDS-Condencyguid-määrite, ennen kuin se tuodaan Azure AD Connectiin. 
  
Lisä tietoja SourceAnchor-ja Condencyguid-tunnuksista on seuraavissa artikkeleissa: [Azure AD Connect: suunnittelu käsitteet](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

