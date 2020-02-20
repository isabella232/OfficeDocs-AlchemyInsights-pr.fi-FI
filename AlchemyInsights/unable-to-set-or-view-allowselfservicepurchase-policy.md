---
title: AllowSelfServicePurchase-käytäntöä ei voi määrittää tai tarkastella
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158558"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>AllowSelfServicePurchase-käytäntöä ei voi määrittää tai tarkastella

Kun yrität määrittää tai tarkastella AllowSelfServicePurchase-käytäntöä, näyttöön tulee seuraava virhesanoma:

*HandleError : Tuotekäytännön noutaminen PolicyId'AllowSelfServicePurchase-, ErrorMessage - Pohjana oleva yhteys katkaistiin: Lähetyksen yhteydessä tapahtui odottamaton virhe.*

Tämä saattaa johtua TLS (Transport Layer Security) -järjestelmän vanhemmasta versiosta. Jos haluat yhdistää MSCommerce-palvelun, sinun on käytettävä TLS 1.2:ta tai uudempaa.  

Ota TLS-protokolla käyttöön tai määritä sen arvoksi 1.2, tarkista ja yritä uudelleen seuraavasti.
 1. Määritä TLS-protokollaversioksi versio\) 1.2 kirjoittamalla PowerShell-komentokehotteeseen (PS C: seuraava komento:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Tarkista käytössä olevat TLS-protokollat seuraavalla komennolla:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Yritä Get- tai Update-komentoja uudelleen tarpeen mukaan.

