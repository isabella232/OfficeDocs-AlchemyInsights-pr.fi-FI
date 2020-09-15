---
title: Virhe Attributevaluempusbesunique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709148"
---
# <a name="error-attributevaluemustbeunique"></a>Virhe: Attributevaluempusbesunique

Yleisin Attributevaluempusbedunique-virheen syy on kaksi objektia, joilla on eri SourceAnchor (immutableId), joilla on sama arvo ProxyAddresses-ja/tai UserPrincipalName-määritteille. Attributevaluempusbedunique-virheen korjaaminen:
  
1. Selvitä virheen aiheuttavan proxyAddresses-, userPrincipalName-tai muun määrite arvon kaksoiskappaleet. Voit myös määrittää, mitkä kaksi (tai useampia) objektia liittyvät risti riitaan. Azure AD Connect Health for Sync-toiminnolla luodun raportin avulla voit tunnistaa nämä kaksi objektia.
    
2. Selvitä, mikä objekti on edelleen päällekkäinen arvo ja mikä objekti ei.
    
3. Poista päällekkäinen arvo objektista, jolla ei pitäisi olla kyseistä arvoa. Huomaa, että sinun on tehtävä muutos siinä hakemistossa, josta objekti on perä isin. Joissain tapa uksissa sinun on ehkä poistettava jokin objekti risti riidasta.
    
4. Jos olet tehnyt muutoksen paikallisessa MAINOKSESSA, anna Azure AD Connectin synkronoida virheen muutos, jotta saat korjattua.
    

