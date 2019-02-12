---
title: DNS-tietueiden päivittäminen sivuston säilyttämiseksi nykyisessä isännöintipalvelussa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: e0dadba1e3ffd1cf0d49c0a76ec2efbbc6ae92db
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906117"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>DNS-tietueiden päivittäminen sivuston säilyttämiseksi nykyisessä isännöintipalvelussa

1. Valitse [Toimialueet](https://portal.office.com/adminportal/home#/Domains) -sivun luettelosta toimialue, jota käytät sivustossasi. Valitse sitten **DNS-asetukset** hallintaruudussa. 
    
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
    

