---
title: Virhekoodi 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jos Virhe otettaessa käyttöön Remote Desktop Services (RDS)-Office-2013, harkitse ADAL käyttöön muokkaamalla rekisteriä.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499379"
---
Jos Virhe otettaessa käyttöön Remote Desktop Services (RDS)-Office-2013, harkitse ADAL käyttöön muokkaamalla rekisteriä. 
  
|**Rekisteriavain**|**Tyyppi**|**Arvo**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1.  <br/> |
   
Lisätietoja [Office 2013 Windows-laitteiden käyttöön Nykyaikainen todennus](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL on käytössä oletusarvoisesti ProPlus Office 365: n ja Office-2016. remote Desktop Services (RDS) > oli ennen nimeltään päätepalvelut. 
  

