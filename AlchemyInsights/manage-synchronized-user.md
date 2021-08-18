---
title: Synkronoidun käyttäjän hallinta
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114775"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Ensisijaisen sähköpostiosoitteen määrittäminen, käyttäjän määritteiden muuttaminen tai synkronoidun käyttäjän poistaminen tai poistaminen ei onnistu

Jos ympäristön hakemistosynkronointi on käytössä, joitakin käyttäjä- tai objektimääritteitä ei voi muuttaa Microsoft 365 -hallintakeskus.

Voit hallita synkronoituja käyttäjiä ja kaikkia niiden määritteitä täydellisesti paikallisilla Active Directory -käyttäjillä ja ryhmien hallintakonsolilla (adsiedit.msc).  

Vaihtoehtoisesti voit muuttaa synkronoitujen käyttäjien yksittäisiä käyttäjiä tai määritteitä PowerShellin avulla, kuten näissä yleisissä esimerkeissä:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
