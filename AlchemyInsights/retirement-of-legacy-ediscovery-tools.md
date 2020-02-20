---
title: Vanhojen eDiscovery-työkalujen eläkkeelle siirtyminen
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
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157572"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Vanhojen eDiscovery-työkalujen eläkkeelle siirtyminen

Microsoft 365 Compliance Centerin uusien ja parannettujen eDiscovery-toimintojen seurauksena seuraavat vanhat eDiscovery-työkalut ja -komennot poistetaan käytöstä tulevina kuukausina:

- [Exchange-hallintakeskuksessa on käytössä eDiscovery-](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) ja [In-Place-pitoja.](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)

- Exchange Online PowerShell -cmdlet-komennot, jotka tukevat in-place eDiscovery- ja In-Place-pitoja. (Nämä cmdlet-komennot tunnistetaan yhteisesti *-MailboxSearch-cmdlet-komennoiksi.) Tämä sisältää seuraavat cmdlet-komennot:

    - [Uusi postilaatikkohaku](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Käynnistä postilaatikkohaku](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch -haku](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Aseta postilaatikkohaku](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Exchange Online PowerShellin [hakupostilaatikon](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet-komento.
- Seuraavat Exchange Web Services -ohjelmointirajapinnan toiminnot:
    - [GetSearchableMailboxes -postilaatikot](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [Aseta HoldOnPostilaatikot](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnPostilaatikot](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Office 365 Advanced eDiscovery v1.0 (Office 365 Advanced eDiscovery v1.0) Office 365 Advanced eDiscovery v1.0](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

**Eläkkeelle siirtymisen aikataulu:**
- 1.4.2020: Et voi luoda uusia hakuja ja pitoja, mutta voit silti suorittaa, muokata ja poistaa olemassa olevia hakuja omalla vastuullasi. Microsoftin tuki ei enää tue EAC:n in Place eDiscovery & -pitoja.

- 1.7.2020: EAC:n in Place eDiscovery & Holds -toiminto sijoitetaan vain luku -tilaan. Tämä tarkoittaa, että voit poistaa vain olemassa olevat haut ja pidot.

**Lisätietoja on kohdassa**:

 - [Vanhojen eDiscovery-hakujen ja -pitojen siirtäminen Microsoft 365 -yhteensopivuuskeskukseen](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Vanhojen eDiscovery-työkalujen eläkkeelle siirtyminen](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Usein kysyttyjä kysymyksiä in-place eDiscovery- ja In-Place-ruuista](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



