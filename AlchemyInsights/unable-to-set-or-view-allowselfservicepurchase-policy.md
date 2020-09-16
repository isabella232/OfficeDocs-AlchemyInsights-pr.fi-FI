---
title: Allowseldo-osto käytäntöä ei voi asettaa tai tarkastella
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735196"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Allowseldo-osto käytäntöä ei voi asettaa tai tarkastella

Näyttöön tulee seuraava virhe sanoma, kun yrität asettaa tai tarkastella Allowselksservicepurchase-käytäntöä:

*HandleError: ei voitu noutaa tuote käytäntöä ja PolicyId ' AllowSelfServicePurchase ', ErrorMessage-perustana oleva yhteys suljettiin: Odottamaton virhe lähetettäessä.*

Tämä voi johtua siitä, että TLS on vanha versio. Jos haluat yhdistää MSCommerce-palvelun, sinun on käytettävä TLS 1,2 tai uudempaa.  

Kokeile seuraavia vaiheita, jos haluat ottaa TLS-protokollan käyttöön tai asettaa sen 1,2, vahvistaa ja yrittää uudelleen.
 1. PowerShell-komento kehotteessa (PS C: \) Kirjoita seuraava komento, jos haluat määrittää TLS-protokollan versioon 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Tarkista käytössä oleva TLS-protokolla ja seuraava komento:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Yritä hakea tai päivittää komentoja tarvittaessa uudelleen.

