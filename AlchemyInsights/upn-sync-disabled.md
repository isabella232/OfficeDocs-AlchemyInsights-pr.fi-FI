---
title: UPN-synkronointi poistettu käytöstä
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
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749511"
---
# <a name="upn-sync-disabled"></a>UPN-synkronointi poistettu käytöstä

Jos aloit synkronoinnin Azure AD:hen ennen 30 päivää maaliskuuta 2016, suorita seuraava Azure AD PowerShell-cmdlet-komento, jotta voit ottaa UPN Soft Match-sovelluksen käyttöön vain organisaatiossa:
  
 **Aseta-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-Ota käyttöön $True**
  
UPN Soft Match-toiminto otetaan automaattisesti käyttöön organisaatioille, jotka aloittivat synkronoinnin Azure AD:hen 2016 maaliskuun 30.
  
Lisä tietoja Soft Match-toiminnon ottamisesta käyttöön UPN:ssä ja muissa synkronointi ominaisuuksissa on artikkelissa [Azure AD Connect-synkronointi palvelun ominaisuudet](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

