---
title: UPN-synkronointi poistettu käytöstä
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
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782148"
---
# <a name="upn-sync-disabled"></a>UPN-synkronointi poistettu käytöstä

Jos aloitit synkronoinnin Azure AD:n kanssa ennen 30. maaliskuuta 2016, suorita seuraava Azure AD PowerShellin cmdlet-komento, jotta voit ottaa käyttöön vain organisaation upn-pehmeän vastineen:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UPN-pehmeä vastaavuus on automaattisesti käytössä organisaatioissa, jotka ovat aloittaneet synkronoinnin Azure AD:n kanssa 30. maaliskuuta 2016 tai sen jälkeen.
  
Lisätietoja pehmeän vastaavuuden ottamalla käyttöön upnissa ja muissa synkronointiominaisuuksissa saat [Azure AD Connect -synkronointipalvelun ominaisuuksista.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

