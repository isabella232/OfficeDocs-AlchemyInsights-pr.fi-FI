---
title: Synkronoitujen käyttäjien hallinta
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541984"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Määritä ensisijainen sähköpostiosoite tai muuta käyttäjän määritteitä ei voi

Jos ympäristössäsi directory-synkronointi on käytössä, käyttäjällä tai objektilla joitakin määritteitä ei voi muuttaa Microsoft 365 hallintakeskukseen.

Voit hallita täysin synkronoitujen käyttäjien ja niiden määritteet, käytä paikallisen active Directoryn käyttäjien ja ryhmien hallintakonsoli (adsiedit.msc-tiedostoa).  

Vaihtoehtoisesti voit muuttaa yksittäisten käyttäjien tai synkronoitu käyttäjät käyttävät näitä yleisiä esimerkkejä kuten näkyy powershell määritteet: 
- Set-MsolUser - UserPrincipalName-user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser - UserPrincipalName ”user@yourdomain.onmicrosoft.com” - DisplayName ”Test käyttäjä” - Sukunimi ”käyttäjä”-osasto ”Manager”-”HR-osasto
- UserPrincipalName - Poista-MsolUser-user@yourdomain.onmicrosoft.com