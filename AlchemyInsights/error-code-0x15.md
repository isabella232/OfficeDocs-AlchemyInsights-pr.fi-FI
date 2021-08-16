---
title: Virhekoodin 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jos saat virhesanoman aktivoitaessa Office 2013 :n Etätyöpöytäpalvelut (RDS) -käyttöönotoissa, harkitse ADAL:n käyttöönottoa muokkaamalla rekisteriä.
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100759"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Virhe aktivoitaessa Office 2013 -palvelua etätyöpöytäpalveluissa

Jos saat virhesanoman aktivoitaessa Office 2013 :n Etätyöpöytäpalvelut (RDS) -käyttöönotoissa, harkitse ADAL:n käyttöönottoa muokkaamalla rekisteriä.
  
|**Rekisteriavain**|**Tyyppi**|**Arvo**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Lisätietoja on kohdassa [Modernin todentamisen ottaminen käyttöön Office 2013 :ssa Windows laitteissa.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
> [!NOTE]
>  ADAL on oletusarvoisesti käytössä Microsoft 365 -sovellukset suuryrityksille Office 2016:ssa. Remote Desktop Services (RDS) oli aiemmin nimeltään Päätepalvelut.
  