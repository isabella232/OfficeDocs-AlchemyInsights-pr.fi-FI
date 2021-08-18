---
title: Virhekoodi 0x15
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
description: Jos saat virhesanoman aktivoitaessa Office 2013 :n etätyöpöytäpalveluiden (RDS) käyttöönotoissa, harkitse ADAL:n käyttöönottoa muokkaamalla rekisteriä.
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316683"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Virhe aktivoitaessa Office 2013 :a etätyöpöytäpalveluissa

Jos saat virhesanoman aktivoitaessa Office 2013 :n etätyöpöytäpalveluiden (RDS) käyttöönotoissa, harkitse ADAL:n käyttöönottoa muokkaamalla rekisteriä.
  
|**Rekisteriavain**|**Tyyppi**|**Arvo**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Lisätietoja on kohdassa [Modernin todentamisen ottaminen käyttöön Office 2013 :ssa Windows laitteissa.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
**Huomautus:** ADAL on oletusarvoisesti käytössä Microsoft 365 -sovellukset suuryrityksille Office 2016:ssa. Remote Desktop Services (RDS) oli aiemmin nimeltään Päätepalvelut.
  