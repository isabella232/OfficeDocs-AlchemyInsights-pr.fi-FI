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
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36526986"
---
# <a name="error-attributevaluemustbeunique"></a>Virhe: AttributeValueMustBeUnique

AttributeValueMustBeUnique-virheen Yleisin syy on kaksi eri SourceAnchor (immutableId) objektien ProxyAddresses- ja UserPrincipalName-määritteiden on sama arvo. Voit korjata virheen AttributeValueMustBeUnique:
  
1. Tunnistaa kaksoiskappaleet proxyAddresses, userPrincipalName tai muita määritteen-arvon, joka aiheuttaa virheen. Tunnistaa myös kahden (tai useamman) mitkä objektit ovat osallisina ristiriita. Raportti Azure AD muodostaa terveys synkronoinnin luoma voi auttaa tunnistamaan kaksi objektia.
    
2. Monistettu arvo olisi edelleen objektin ja objektin ei tulisi tunnistaa.
    
3. Poista objekti, joka ei saa olla arvon kopioidun arvon. Huomaa, että olisi muutoksen missä objekti Orpotermit-hakemistossa. Joissakin tapauksissa joudut ehkä poistaa ristiriitaiset objektit.
    
4. Jos AD tiloissa on tehty muutos, anna Azure synkronoinnin virhe on korjattu muutos AD-muodosta.
    

