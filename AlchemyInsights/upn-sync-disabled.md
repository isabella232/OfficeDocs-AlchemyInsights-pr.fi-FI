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
# <a name="upn-sync-disabled"></a><span data-ttu-id="c91bb-102">UPN-synkronointi poistettu käytöstä</span><span class="sxs-lookup"><span data-stu-id="c91bb-102">UPN sync disabled</span></span>

<span data-ttu-id="c91bb-103">Jos aloitit synkronoinnin Azure AD:n kanssa ennen 30. maaliskuuta 2016, suorita seuraava Azure AD PowerShellin cmdlet-komento, jotta voit ottaa käyttöön vain organisaation upn-pehmeän vastineen:</span><span class="sxs-lookup"><span data-stu-id="c91bb-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="c91bb-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span><span class="sxs-lookup"><span data-stu-id="c91bb-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="c91bb-105">UPN-pehmeä vastaavuus on automaattisesti käytössä organisaatioissa, jotka ovat aloittaneet synkronoinnin Azure AD:n kanssa 30. maaliskuuta 2016 tai sen jälkeen.</span><span class="sxs-lookup"><span data-stu-id="c91bb-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="c91bb-106">Lisätietoja pehmeän vastaavuuden ottamalla käyttöön upnissa ja muissa synkronointiominaisuuksissa saat [Azure AD Connect -synkronointipalvelun ominaisuuksista.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)</span><span class="sxs-lookup"><span data-stu-id="c91bb-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

