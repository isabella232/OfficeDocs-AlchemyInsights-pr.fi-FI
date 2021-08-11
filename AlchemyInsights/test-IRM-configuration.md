---
title: IRM-määritysten testaaminen uusille OME-ominaisuuksille
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812434"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>IRM-määritysten testaaminen uusille OME-ominaisuuksille

Varmista, että Microsoft 365 on määritetty käyttämään uusia OME-ominaisuuksia, kun muodostat yhteyden [PowerShelliin Exchange Online cmdlet-komennoilla:](/powershell/exchange/exchange-online-powershell)


1. Tarkista vuokraajan IRM-määritykset suorittamalla `Get-IRMConfiguration` . Varmista, että näiden arvojen arvoksi on määritetty **Tosi:**
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Suorita toimialue, lähettäjän osoite ja vastaanottajan `Test-IRMConfiguration` avulla. Jos testi ei läpäise, tutki IRM-määritystä.

Lisätietoja IRM-määritysten tarkistamista varten on kohdassa Uusien [OME-määritysten tarkistaminen Exchange Online PowerShellissä.](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)