---
title: Virhekoodi 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jos saat virheilmoituksen aktivoidessasi Office 2013:n etätyöpöytäpalveluiden (RDS) käyttöönotoissa, harkitse ADAL-joukkojen käyttöönottoa muokkaamalla rekisteriä.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506843"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Virhe aktivoitaessa Office 2013:a etätyöpöytäpalveluissa

Jos saat virheilmoituksen aktivoidessasi Office 2013:n etätyöpöytäpalveluiden (RDS) käyttöönotoissa, harkitse ADAL-joukkojen käyttöönottoa muokkaamalla rekisteriä.
  
|**Rekisteriavain**|**Tyyppi**|**Arvo**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Lisätietoja on ohjeaiheessa [Office 2013:n nykyaikaisen todennuksen ottaminen käyttöön Windows-laitteissa](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL on oletusarvoisesti käytössä Microsoft 365 Apps for Enterprisessa ja Office 2016:ssa. Etätyöpöytäpalvelut (RDS) nimettiin aiemmin päätepalveluille.
  