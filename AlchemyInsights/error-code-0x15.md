---
title: Virhe koodi 0x15
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
description: 'Jos saat virhe ilmoituksen, kun Akti voit Office 2013: n Etätyöpöytäpalvelujen (RDS) käyttöönotoissa, harkitse ADALIN ottamista käyttöön muokkaamalla rekisteriä.'
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709184"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Virhe Office 2013-sovelluksen Akti voinnin yhteydessä Etätyöpöytäpalveluissa

Jos saat virhe ilmoituksen, kun Akti voit Office 2013: n Etätyöpöytäpalvelujen (RDS) käyttöönotoissa, harkitse ADALIN ottamista käyttöön muokkaamalla rekisteriä.
  
|**Rekisteriavain**|**Tyyppi**|**Arvo**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\microsoft\office\15.0\common\identyt\enableadal  <br/> |REG_DWORD  <br/> |1  <br/> |

Lisä tietoja on Ohje aiheessa [Office 2013: n modernin todennuksen ottaminen käyttöön Windows-laitteissa](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL on oletusarvoisesti käytössä Microsoft 365-sovelluksissa yritys käyttöön ja Office 2016-sovellukseen. Etätyöpöytä palvelut (RDS) nimettiin aiemmin pääte palveluina.
  