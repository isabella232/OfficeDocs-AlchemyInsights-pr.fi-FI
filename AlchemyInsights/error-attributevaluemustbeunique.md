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
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7b98b68fabff6c048f1bab6cf506355114d18658
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916521"
---
# <a name="error-attributevaluemustbeunique"></a>Virhe: AttributeValueMustBeUnique

AttributeValueMustBeUnique-virheen Yleisin syy on kaksi eri SourceAnchor (immutableId) objektien ProxyAddresses- ja UserPrincipalName-määritteiden on sama arvo. Voit korjata virheen AttributeValueMustBeUnique:
  
1. Tunnistaa kaksoiskappaleet proxyAddresses, userPrincipalName tai muita määritteen-arvon, joka aiheuttaa virheen. Tunnistaa myös kahden (tai useamman) mitkä objektit ovat osallisina ristiriita. Raportti Azure AD muodostaa terveys synkronoinnin luoma voi auttaa tunnistamaan kaksi objektia.
    
2. Monistettu arvo olisi edelleen objektin ja objektin ei tulisi tunnistaa.
    
3. Poista objekti, joka ei saa olla arvon kopioidun arvon. Huomaa, että olisi muutoksen missä objekti Orpotermit-hakemistossa. Joissakin tapauksissa joudut ehkä poistaa ristiriitaiset objektit.
    
4. Jos AD tiloissa on tehty muutos, anna Azure synkronoinnin virhe on korjattu muutos AD-muodosta.
    

