---
title: DNS-tietueiden päivittäminen sivuston säilyttämiseksi nykyisessä isännöintipalvelussa
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815782"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>DNS-tietueiden päivittäminen sivuston säilyttämiseksi nykyisessä isännöintipalvelussa

1. Siirry Microsoft 365-hallinta keskuksessa **Määritä**toimi  >  [alueet](https://admin.microsoft.com/Adminportal#/Domains) -sivulle ja valitse toimi alue luettelosta sivusto, jota käytät sivustossasi.

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
