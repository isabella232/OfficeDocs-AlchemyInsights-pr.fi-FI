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
ms.openlocfilehash: f868ce25d68f61da30d2db4de88aa83675c97857b3c1371cf2039e0b03895a64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007679"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>DNS-tietueiden päivittäminen sivuston säilyttämiseksi nykyisessä isännöintipalvelussa

1. Siirry Microsoft 365 -hallintakeskus Toimialueiden määritys -sivulle ja valitse toimialueiden luettelosta toimialue, jonka avulla   >  [](https://admin.microsoft.com/Adminportal#/Domains) käytät sivustoasi.

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
