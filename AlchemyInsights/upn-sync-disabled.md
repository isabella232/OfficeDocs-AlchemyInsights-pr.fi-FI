---
title: UPN-synkronointi on poistettu käytöstä
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: d00f10688ec775c22d60a9089e291c265ada46f1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29467650"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="e38ed-102">UPN-synkronointi on poistettu käytöstä</span><span class="sxs-lookup"><span data-stu-id="e38ed-102">UPN sync disabled</span></span>

<span data-ttu-id="e38ed-103">Jos käynnistit Azure AD 30. maaliskuuta 2016 ennen synkronointi suoritetaan UPN Pehmeä vastaavat vain organisaation käyttöön seuraavat Azure AD PowerShellin cmdlet-komennolla:</span><span class="sxs-lookup"><span data-stu-id="e38ed-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="e38ed-104">**Set-MsolDirSyncFeature-ominaisuus on EnableSoftMatchOnUpn-$True käyttöön**</span><span class="sxs-lookup"><span data-stu-id="e38ed-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="e38ed-105">UPN-Pehmeä vastine otetaan automaattisesti käyttöön organisaatioille, jotka aloittaa synkronoinnin Azure AD aikaisintaan 30. maaliskuuta 2016.</span><span class="sxs-lookup"><span data-stu-id="e38ed-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="e38ed-106">Lisätietoja Pehmeä vastine UPN ja synkronointi muiden ominaisuuksien ottaminen käyttöön lisätietoja [Azure AD muodosta synkronointi palvelun ominaisuuksia](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="e38ed-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

