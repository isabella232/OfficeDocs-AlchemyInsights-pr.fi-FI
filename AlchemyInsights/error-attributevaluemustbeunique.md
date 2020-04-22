---
title: Virhe AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: fa1fdb35f1af250bc98aa61c0e5111f1f1b8aac4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703171"
---
# <a name="error-attributevaluemustbeunique"></a>Virhe: AttributeValueMustBeUnique

Suurin syy AttributeValueValueMustBeUnique-virheeseen on kaksi objektia, joilla on eri SourceAnchor (immutableId) -arvo ProxyAddresses- ja/tai UserPrincipalName-määritteille. Voit korjata AttributeValueValueBeUnique-virheen seuraavasti:
  
1. Määritä päällekkäiset proxyAddresses-osoitteet, userPrincipalName tai muu määritteen arvo, joka aiheuttaa virheen. Selvitä myös, mitkä kaksi (tai useampia) objekteja liittyy konfliktiin. Azure AD Connect Healthin synkronoitavaksi luoma raportti voi auttaa tunnistamaan nämä kaksi objektia.
    
2. Määritä, millä objektilla on edelleen kaksoiskappalearvo ja mikä objekti ei saa olla.
    
3. Poista kaksoiskappalearvo objektista, jolla EI pitäisi olla kyseistä arvoa. Huomaa, että sinun on tehtävä muutos hakemistoon, josta objekti on peräisin. Joissakin tapauksissa saatat joutua poistamaan jonkin ristiriitaisista objekteista.
    
4. Jos teit muutoksen paikallisessa AD:ssä, anna Azure AD Connectin synkronoida virheen korjaaminen.
    

