---
title: AllowSelfServicePurchase-käytännön joukon tai tarkasteleminen ei onnistu
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
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826088"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>AllowSelfServicePurchase-käytännön joukon tai tarkasteleminen ei onnistu

Kun yrität määrittää tai tarkastella AllowSelfServicePurchase-käytäntöä, näyttöön tulee seuraava virhesanoma:

*HandleError: Tuotekäytännön noutaminen epäonnistui, kun PolicyId on AllowSelfServicePurchase, ErrorMessage - Pohjana oleva yhteys suljettiin: Lähetystä käsiteltäessä tapahtui odottamaton virhe.*

Tämä voi johtua TLS (Transport Layer Security) -suojausversion vanhemman version vuoksi. Jos haluat yhdistää MSCommerce-palvelun, sinun on käytettävä TLS 1.2:ta tai sitä uudempia.  

Seuraavien vaiheiden avulla voit ottaa TLS-protokollan käyttöön tai määrittää sen arvoksi 1.2, tarkistaa ja yrittää uudelleen.
 1. Määritä TLS-protokolla versioksi 1.2 kirjoittamalla PowerShell-komentokehotteeseen (PS C: määritä \) TLS-protokolla versioon 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Varmista, että TLS-protokollat ovat käytössä, seuraavalla komennolla:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Yritä tarvittaessa Hae- tai Päivitä-komentoja uudelleen.

