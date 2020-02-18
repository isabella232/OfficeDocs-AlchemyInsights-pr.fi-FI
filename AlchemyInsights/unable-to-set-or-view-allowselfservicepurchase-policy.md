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
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091694"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>AllowSelfServicePurchase-käytäntöä ei voi määrittää tai tarkastella

Kun yrität määrittää tai tarkastella AllowSelfServicePurchase-käytäntöä, näyttöön tulee seuraava virhesanoma:

*HandleError : Tuotekäytännön noutaminen PolicyId'AllowSelfServicePurchase-, ErrorMessage - Pohjana oleva yhteys katkaistiin: Lähetyksen yhteydessä tapahtui odottamaton virhe.*

Tämä saattaa johtua TLS (Transport Layer Security) -järjestelmän vanhemmasta versiosta. Jos haluat yhdistää MSCommerce-palvelun, sinun on käytettävä TLS 1.2:ta tai uudempaa.  

Ota TLS-protokolla käyttöön tai määritä sen arvoksi 1.2, tarkista ja yritä uudelleen seuraavasti.
 1. Määritä TLS-protokollaversioksi versio\) 1.2 kirjoittamalla PowerShell-komentokehotteeseen (PS C: seuraava komento:

    \[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12

2. Tarkista käytössä olevat TLS-protokollat seuraavalla komennolla:

    \[Net.ServicePointManager]::Suojausprotokolla 

3. Yritä Get- tai Update-komentoja uudelleen tarpeen mukaan.

