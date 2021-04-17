---
title: DNS-tietueiden päivittäminen sivuston säilyttämiseksi nykyisessä isännöintipalvelussa
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827512"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>DNS-tietueiden päivittäminen sivuston säilyttämiseksi nykyisessä isännöintipalvelussa

1. Siirry Microsoft 365 -hallintakeskuksessa Määritä toimialueet -sivulle ja valitse toimialueiden luettelosta toimialue, jossa käytät  >  [](https://admin.microsoft.com/Adminportal#/Domains) sivustoasi.

2. Valitse **+ Uusi mukautettu tietue** ja anna seuraavat tiedot:

  - Määritä **DNS-tyyppi**: **A (osoite)**

  - Kirjoita **Isäntänimi tai alias** -kohtaan **@**

  - Kirjoita **IP-osoite** -kohtaan muualla isännöidyn sivustosi staattinen IP-osoite, esimerkiksi 172.16.140.1.

    Sivuston osoitteen on oltava  *staattinen*  IP-osoite, ei  *dynaaminen*  IP-osoite. Tarkista sivustosi isännöintipalvelusta, voitko saada käyttöön staattisen IP-osoitteen julkista sivustoasi varten.

3. Valitse **Tallenna**.

Voit halutessasi luoda myös CNAME-tietueen, joka auttaa asiakkaita löytämään sivuston.
  
1. Valitse **+ Uusi mukautettu tietue** ja anna seuraavat tiedot:

  - Määritä **DNS-tyyppi**: **CNAME (alias)**

  - Kirjoita **Isäntänimi tai alias** -kohtaan **www**

  - Kirjoita **Kohdeosoite** -kohtaan sivuston täydellinen toimialuenimi, esimerkiksi contoso.com.

2. Valitse **Tallenna**.
