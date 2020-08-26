---
title: Vanhojen eDiscoveryn poistaminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902617"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Vanhojen eDiscoveryn poistaminen

Microsoft 365-yhteensopivuus keskuksen uusien ja parannettujen eDiscoveryn toimintojen tuloksena seuraavat vanhat eDiscoveryn työkalut ja komentosovelmat poistuvat käytöstä lähikuukausina:

- Exchange-hallinta keskuksen käytössä oleva [etsimis](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) -ja pito [paikka](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) .

- Exchange Online PowerShellin cmdlet-komentosovelmat, jotka tukevat sijaintia etsimis-ja paikallaan. (Nämä cmdlet-komentosovelmat tunnistetaan yhteisesti *-posti laatikon haun cmdlet-komentosovelmat.) Tämä sisältää seuraavat cmdlet-komento:

    - [Uusi-Mailposti-haku](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Käynnistä-posti laatikon haku](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Pysäytä-posti laatikon haku](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Asetukset-posti laatikon haku](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [Search-Mailbox-cmdlet-](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) vaihto Exchange Online PowerShellissä.
- Seuraavat Exchange Web Services-ohjelmointi raja pinnan toiminnot:
    - [Getsearchtablemailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [Asetholdonposti laatikot](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [Geosholdonpostilaatikkoposti laatikot](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscoveryn v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Eläkkeelle siirtymisen aika Jana**:
- **1. heinä kuuta 2020** Et voi enää luoda uusia hakuja ja pitää niitä, mutta voit suorittaa, muokata ja poistaa olemassa olevia hakuja omalla vastuullasi. Microsoft-tuki ei enää tue paikan päällä olevaa eDiscoverya & pätee EAC:ssä.
    
- **1. loka kuuta, 2020** Paikan päällä oleva eDiscoveryn &-toiminto on käytettävissä vain luku-tilassa, joten voit poistaa vain olemassa olevat haut ja ruumat.

Lisä **tietoja on kohdassa**:

 - [Vanhojen eDiscoveryn hakujen ja Pitojen siirtäminen Microsoft 365-yhteensopivuus keskukseen](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Vanhojen eDiscoveryn poistaminen](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Usein kysyttyjä kysymyksiä paikasta ja paikasta](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



