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
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038109"
---
# <a name="upn-sync-disabled"></a>UPN-synkronointi poistettu käytöstä

Jos aloitit synkronoinnin Azure AD:n kanssa ennen 30. maaliskuuta 2016, suorita seuraava Azure AD PowerShellin cmdlet-komento, jotta voit ottaa käyttöön vain organisaation upn-pehmeän vastineen:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UPN-pehmeä vastaavuus on automaattisesti käytössä organisaatioissa, jotka ovat aloittaneet synkronoinnin Azure AD:n kanssa 30. maaliskuuta 2016 tai sen jälkeen.
  
Lisätietoja pehmeän vastaavuuden ottamalla käyttöön upnissa ja muissa synkronointiominaisuuksissa on [kohdassa Azure AD Näyttöyhteys synkronointipalvelun ominaisuudet.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

