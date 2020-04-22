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
description: Jos saat virheilmoituksen aktivoidessasi Office 2013:n etätyöpöytäpalveluiden (RDS) käyttöönotoissa, ota ADAL käyttöön muokkaamalla rekisteriä.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703135"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Virhe aktivoitaessa Office 2013:a etätyöpöytäpalveluissa

Jos saat virheilmoituksen aktivoidessasi Office 2013:n etätyöpöytäpalveluiden (RDS) käyttöönotoissa, ota ADAL käyttöön muokkaamalla rekisteriä.
  
|**Rekisteriavain**|**Tyyppi**|**Arvo**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |Reg_dword  <br/> |1  <br/> |

Lisätietoja on ohjeaiheessa [Nykyaikaisen todennuksen ottaminen käyttöön Office 2013:ssa Windows-laitteissa](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL on oletusarvoisesti käytössä Microsoft 365 Apps for Enterprise- ja Office 2016 -sovelluksissa. Etätyöpöytäpalvelut (RDS) nimettiin aiemmin päätepalveluiksi.
  