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
# <a name="upn-sync-disabled"></a><span data-ttu-id="c1bdb-102">UPN-synkronointi poistettu käytöstä</span><span class="sxs-lookup"><span data-stu-id="c1bdb-102">UPN sync disabled</span></span>

<span data-ttu-id="c1bdb-103">Jos aloit synkronoinnin Azure AD:hen ennen 30 päivää maaliskuuta 2016, suorita seuraava Azure AD PowerShell-cmdlet-komento, jotta voit ottaa UPN Soft Match-sovelluksen käyttöön vain organisaatiossa:</span><span class="sxs-lookup"><span data-stu-id="c1bdb-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="c1bdb-104">**Aseta-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-Ota käyttöön $True**</span><span class="sxs-lookup"><span data-stu-id="c1bdb-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="c1bdb-105">UPN Soft Match-toiminto otetaan automaattisesti käyttöön organisaatioille, jotka aloittivat synkronoinnin Azure AD:hen 2016 maaliskuun 30.</span><span class="sxs-lookup"><span data-stu-id="c1bdb-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="c1bdb-106">Lisä tietoja Soft Match-toiminnon ottamisesta käyttöön UPN:ssä ja muissa synkronointi ominaisuuksissa on artikkelissa [Azure AD Connect-synkronointi palvelun ominaisuudet](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="c1bdb-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

