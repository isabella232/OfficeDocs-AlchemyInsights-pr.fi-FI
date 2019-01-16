---
title: 932 päivittämistä AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9add88a0e4a2590639cbfc546afdcdf5e6aa4886
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28287179"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="c6ed8-102">Yhdistä päivityksen Azure AD</span><span class="sxs-lookup"><span data-stu-id="c6ed8-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="c6ed8-p101">Oletusarvon mukaan Automaattinen päivitys on käytössä Azure AD muodosta, jonka avulla voit varmistaa käytössä uusin versio. Avulla voit varmistaa automaattisen päivityksen asetuksia, Azure AD PowerShellin **Get-ADSyncAutoUpgrade** -cmdlet-komennolla. Palauttaa cmdlet jokin seuraavista arvoista:</span><span class="sxs-lookup"><span data-stu-id="c6ed8-p101">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version. To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell. The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="c6ed8-106">**Käytössä**: Automaattinen päivitys on käytössä.</span><span class="sxs-lookup"><span data-stu-id="c6ed8-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="c6ed8-107">**Poistettu käytöstä**: Automaattinen päivitys on poistettu käytöstä.</span><span class="sxs-lookup"><span data-stu-id="c6ed8-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="c6ed8-p102">**Suspended**: Järjestelmä ei ole enää oikeutettu saamaan Automaattiset päivitykset. Et voi määrittää tämän arvon. se määritetään järjestelmä.</span><span class="sxs-lookup"><span data-stu-id="c6ed8-p102">**Suspended**: The system is no longer eligible to receive automatic upgrades. You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="c6ed8-110">Lisätietoja [automaattisen päivityksen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="c6ed8-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="c6ed8-111">Voit ladata uusimman version Azure AD-muodosta, [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="c6ed8-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

