---
title: Välityspalvelimen osoitevirhe jaetun postilaatikon luonnin aikana
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568287"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Välityspalvelimen osoitevirhe luotaessa postilaatikkoa tai muuta sähköpostia käyttävää objektia

Jos yritit luoda sähköpostia käyttävän objektin (postilaatikko, jaettu postilaatikko jne.) ja sait virhesanoman "Välityspalvelimen osoite "SMTP:alias@domain.com" on jo käytössä...", valitsemasi sähköpostiosoite on jo toisen organisaation sähköpostia käyttävän objektin käytössä.
  
Sinun on etsittava käyttäjä, ryhmä, jaettu postilaatikko tai yleinen kansio, jossa tämä sähköpostiosoite on, ja poistettava se tai muutettava sen sähköpostiosoitetta. Sen jälkeen voit luoda uuden sähköpostia käyttävän objektin, jossa on vapaita sähköpostiosoitteita. Etsi se aloitussivun Haku-haun avulla. Voit etsiä sitä myös seuraavan Exchange Online PowerShell -komennon avulla:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Jos et halua poistaa olemassa olevaa sähköpostiosoitetta, valitse uusi sähköpostiosoite luomallesi uudelle objektille.
  