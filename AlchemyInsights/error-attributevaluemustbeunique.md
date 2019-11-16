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
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/15/2019
ms.locfileid: "36526986"
---
# <a name="error-attributevaluemustbeunique"></a>Virhe: AttributeValueMustBeUnique

AttributeValueMustBeUnique-virheen yleisin syy on kaksi objektia, joilla on eri SourceAnchor (immutableId), on sama arvo Proxyosoitteet-ja/tai UserPrincipalName-määritteillä. Voit korjata AttributeValueMustBeUnique-virheen:
  
1. Tunnista kopioitu Proxyosoitteet, userPrincipalName tai muu määritteen arvo, joka aiheuttaa virheen. Selvitä myös, mitkä kaksi (tai useampia) objektia on osallisena konfliktissa. Azure AD Connect Health for Sync-ohjelman luoma raportti voi auttaa tunnistamaan kaksi objektia.
    
2. Määritä, minkä objektin kaksoisarvon on oltava, ja mitä objektia ei pitäisi käyttää.
    
3. Poista kopioitu arvo objektista, jolla ei ole kyseistä arvoa. Huomaa, että sinun tulee tehdä muutos hakemistoon, josta objekti on perä isin. Joissakin tapa uksissa saatat joutua poistamaan jonkin risti riidassa olevasta objektista.
    
4. Jos olet tehnyt muutoksen paikallisessa MAINOKSESSA, anna Azure AD Connectin synkronoida virheen muutos, jotta saat kiinteän.
    

