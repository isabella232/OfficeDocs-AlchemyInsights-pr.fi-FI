---
title: Virhe AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7fc1190fb7b93dce945e366cf8b90112a97a2f3f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402700"
---
# <a name="error-attributevaluemustbeunique"></a>Virhe: AttributeValueMustBeUnique

AttributeValueMustBeUnique-virheen Yleisin syy on kaksi eri SourceAnchor (immutableId) objektien ProxyAddresses- ja UserPrincipalName-määritteiden on sama arvo. Voit korjata virheen AttributeValueMustBeUnique:
  
1. Tunnistaa kaksoiskappaleet proxyAddresses, userPrincipalName tai muita määritteen-arvon, joka aiheuttaa virheen. Tunnistaa myös kahden (tai useamman) mitkä objektit ovat osallisina ristiriita. Raportti Azure AD muodostaa terveys synkronoinnin luoma voi auttaa tunnistamaan kaksi objektia.
    
2. Monistettu arvo olisi edelleen objektin ja objektin ei tulisi tunnistaa.
    
3. Poista objekti, joka ei saa olla arvon kopioidun arvon. Huomaa, että olisi muutoksen missä objekti Orpotermit-hakemistossa. Joissakin tapauksissa joudut ehkä poistaa ristiriitaiset objektit.
    
4. Jos AD tiloissa on tehty muutos, anna Azure synkronoinnin virhe on korjattu muutos AD-muodosta.
    

