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
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823964"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Ensisijaisen sähköpostiosoitteen määrittäminen, käyttäjän määritteiden muuttaminen tai synkronoidun käyttäjän poistaminen tai poistaminen ei onnistu

Jos hakemistosynkronointi on käytössä ympäristössäsi, joitakin käyttäjä- tai objektimääritteitä ei voi muuttaa Microsoft 365 -hallintakeskuksen avulla.

Voit hallita synkronoituja käyttäjiä ja kaikkia niiden määritteitä täydellisesti paikallisilla Active Directory -käyttäjillä ja ryhmien hallintakonsolilla (adsiedit.msc).  

Vaihtoehtoisesti voit muuttaa synkronoitujen käyttäjien yksittäisiä käyttäjiä tai määritteitä PowerShellin avulla, kuten näissä yleisissä esimerkeissä:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
