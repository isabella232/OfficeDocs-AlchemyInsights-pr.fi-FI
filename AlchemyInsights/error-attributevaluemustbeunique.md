---
title: Virhe AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7a97d1a5ff352b55833bd457e3220a56130d7e7e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28286997"
---
# <a name="error-attributevaluemustbeunique"></a>Virhe: AttributeValueMustBeUnique

AttributeValueMustBeUnique-virheen Yleisin syy on kaksi eri SourceAnchor (immutableId) objektien ProxyAddresses- ja UserPrincipalName-määritteiden on sama arvo. Voit korjata virheen AttributeValueMustBeUnique:
  
1. Tunnistaa kaksoiskappaleet proxyAddresses, userPrincipalName tai muita määritteen-arvon, joka aiheuttaa virheen. Tunnistaa myös kahden (tai useamman) mitkä objektit ovat osallisina ristiriita. Raportti Azure AD muodostaa terveys synkronoinnin luoma voi auttaa tunnistamaan kaksi objektia.
    
2. Monistettu arvo olisi edelleen objektin ja objektin ei tulisi tunnistaa.
    
3. Poista objekti, joka ei saa olla arvon kopioidun arvon. Huomaa, että olisi muutoksen missä objekti Orpotermit-hakemistossa. Joissakin tapauksissa joudut ehkä poistaa ristiriitaiset objektit.
    
4. Jos AD tiloissa on tehty muutos, anna Azure synkronoinnin virhe on korjattu muutos AD-muodosta.
    

