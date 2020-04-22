---
title: UPN-synkronointi poistettu käytöstä
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
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726101"
---
# <a name="upn-sync-disabled"></a>UPN-synkronointi poistettu käytöstä

Jos aloitit synkronoinnin Azure AD:hen ennen 30.3.2016, ota UPN:n pehmeä vastaavuus käyttöön vain organisaatiossa suorittamalla seuraava Azure AD PowerShell -cmdlet-komento:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Ota $True**
  
UPN:n pehmeä ottelu otetaan automaattisesti käyttöön organisaatioissa, jotka aloittivat synkronoinnin Azure AD:hen 30.3.2016 tai sen jälkeen.
  
Lisätietoja upn-toiminnon ja muiden synkronointiominaisuuksien ottamisesta käyttöön on kohdassa [Azure AD Connect -synkronointipalvelun ominaisuudet](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

