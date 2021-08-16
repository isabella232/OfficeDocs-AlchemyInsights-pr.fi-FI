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
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002117"
---
# <a name="error-attributevaluemustbeunique"></a>Virhe: AttributeValueMustBeUnique

AttributeValueMustBeUnique-virheen yleisin syy on se, että kahdella SourceAnchor-objektilla (immutableId) on sama arvo ProxyAddresses- ja/tai UserPrincipalName-määritteissä. AttributeValueMustBeUnique-virheen ratkaiseminen:
  
1. Tunnista proxyAddresses-, userPrincipalName- tai muu määritearvo, joka aiheuttaa virheen. Määritä myös, mitkä kaksi objektia (tai enemmän) ovat ristiriidassa. Azure AD Näyttöyhteys Health for Syncin luoma raportti auttaa tunnistamaan kaksi objektia.
    
2. Määritä, millä objektilla pitäisi edelleen olla kaksoiskappalearvo ja minkä objektin ei pitäisi olla.
    
3. Poista kaksoiskappale objektista, jossa EI pitäisi olla tätä arvoa. Huomaa, että sinun tulisi tehdä muutos hakemistoon, josta objekti on peräisin. Joissakin tapauksissa sinun on ehkä poistettava jokin ristiriitainen objekti.
    
4. Jos teit muutoksen paikallisissa AD-ilmoituksissa, anna Azure AD Näyttöyhteys synkronoida virheen muutos, jotta se korjautuu.
    

