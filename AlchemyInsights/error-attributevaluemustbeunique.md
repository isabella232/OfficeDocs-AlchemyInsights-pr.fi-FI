---
title: Error AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813757"
---
# <a name="error-attributevaluemustbeunique"></a>Virhe: AttributeValueMustBeUnique

AttributeValueMustBeUnique-virheen yleisin syy on se, että kahdella SourceAnchor-objektilla (immutableId) on sama arvo ProxyAddresses- ja/tai UserPrincipalName-määritteissä. AttributeValueMustBeUnique-virheen ratkaiseminen:
  
1. Tunnista proxyAddresses-, userPrincipalName- tai muu määritearvo, joka aiheuttaa virheen. Määritä myös, mitkä kaksi objektia (tai enemmän) ovat ristiriidassa. Azure AD Connect Healthin synkronointia varten luoman raportin avulla voit tunnistaa kaksi objektia.
    
2. Määritä, millä objektilla pitäisi edelleen olla kaksoiskappalearvo ja minkä objektin ei pitäisi olla.
    
3. Poista kaksoiskappale objektista, jossa EI pitäisi olla tätä arvoa. Huomaa, että sinun tulisi tehdä muutos hakemistoon, josta objekti on peräisin. Joissakin tapauksissa sinun on ehkä poistettava jokin ristiriitainen objekti.
    
4. Jos teit muutoksen paikallisissa AD-ilmoituksissa, anna Azure AD Connectin synkronoida virheen muutos, jotta se korjautuu.
    

