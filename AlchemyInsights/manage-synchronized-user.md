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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380502"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Määritä ensisijainen sähköpostiosoite tai muuta käyttäjän määritteitä ei voi

Jos hakemiston synkronointi on käytössä ympäristössäsi käyttäjällä tai objektilla joitakin määritteitä ei voi muuttaa hallintakeskukseen.
Voit hallita täysin synkronoitujen käyttäjien ja niiden määritteet, käytä paikallisen active Directoryn käyttäjien ja ryhmien hallintakonsoli (adsiedit.msc-tiedostoa).  

Vaihtoehtoisesti voit muuttaa yksittäisten käyttäjien tai synkronoitu käyttäjät käyttävät näitä yleisiä esimerkkejä kuten näkyy powershell määritteet: 
- Set-MsolUser - UserPrincipalName-user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser - UserPrincipalName ”user@yourdomain.onmicrosoft.com” - DisplayName ”Test käyttäjä” - Sukunimi ”käyttäjä”-osasto ”Manager”-”HR-osasto
- UserPrincipalName - Poista-MsolUser-user@yourdomain.onmicrosoft.com