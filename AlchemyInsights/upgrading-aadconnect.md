---
title: 932 päivittämistä AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 0bbb847bb1381330065ebba6e109795908b06490
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/22/2019
ms.locfileid: "30778739"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="d754e-102">Yhdistä päivityksen Azure AD</span><span class="sxs-lookup"><span data-stu-id="d754e-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="d754e-103">Oletusarvon mukaan Automaattinen päivitys on käytössä Azure AD muodosta, jonka avulla voit varmistaa käytössä uusin versio.</span><span class="sxs-lookup"><span data-stu-id="d754e-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="d754e-104">Avulla voit varmistaa automaattisen päivityksen asetuksia, Azure AD PowerShellin **Get-ADSyncAutoUpgrade** -cmdlet-komennolla.</span><span class="sxs-lookup"><span data-stu-id="d754e-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="d754e-105">Palauttaa cmdlet jokin seuraavista arvoista:</span><span class="sxs-lookup"><span data-stu-id="d754e-105">The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="d754e-106">**Käytössä**: Automaattinen päivitys on käytössä.</span><span class="sxs-lookup"><span data-stu-id="d754e-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="d754e-107">**Poistettu käytöstä**: Automaattinen päivitys on poistettu käytöstä.</span><span class="sxs-lookup"><span data-stu-id="d754e-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="d754e-108">**Suspended**: Järjestelmä ei ole enää oikeutettu saamaan Automaattiset päivitykset.</span><span class="sxs-lookup"><span data-stu-id="d754e-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="d754e-109">Et voi määrittää tämän arvon. se määritetään järjestelmä.</span><span class="sxs-lookup"><span data-stu-id="d754e-109">You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="d754e-110">Lisätietoja [automaattisen päivityksen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="d754e-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="d754e-111">Voit ladata uusimman version Azure AD-muodosta, [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="d754e-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

