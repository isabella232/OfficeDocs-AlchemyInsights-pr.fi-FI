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
ms.openlocfilehash: 262cca0feee17d1f929a5a94a4dd6c1ec317f6ec
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/21/2020
ms.locfileid: "43650565"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Vanhojen eDiscovery-työkalujen eläkkeelle siirtyminen

Microsoft 365 Compliance Centerin uusien ja parannettujen eDiscovery-toimintojen ansiosta seuraavat vanhat eDiscovery-työkalut ja komentokomennot poistetaan lähikuukausina:

- [Exchange-hallintakeskuksessa on käytössä eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) ja [in-place-pito.](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)

- Exchange Online PowerShell -cmdlet-komennot, jotka tukevat in-place eDiscovery- ja in-Place Holds -komentoja. (Nämä cmdlet-komennot tunnistetaan yhdessä *-MailboxSearch-cmdlet-komennoiksi.) Tämä sisältää seuraavat cmdlet-komennot:

    - [Uusi mailboxsearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Aloita postilaatikon haku](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxHaku](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Aseta-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [Exchange](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) Online PowerShellin Search-Mailbox-cmdlet-komento.
- Seuraavat Exchange Web Services -ohjelmointirajapinnan toiminnot:
    - [GetSearchableMailboxes -kohteet](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes-kohteet](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes -kohteet](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Kehittynyt eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Eläkkeelle siirtymisen aikataulu**:
- 1.4.2020: Et voi luoda uusia hakuja ja pitoja, mutta voit silti suorittaa, muokata ja poistaa olemassa olevia hakuja omalla vastuullasi. Microsoftin tuki ei enää tue EAC:n in-Place eDiscovery & Holds -&.

- 1.7.2020: EDiscovery & Holds -toiminto eAC:ssä sijoitetaan vain luku -tilaan. Tämä tarkoittaa, että voit poistaa vain olemassa olevat haut ja pidot.

**Lisätietoja on kohdassa**:

 - [Vanhojen eDiscovery-hakujen ja pitotietojen siirtäminen Microsoft 365 -yhteensopivuuskeskukseen](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Vanhojen eDiscovery-työkalujen eläkkeelle siirtyminen](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Usein kysyttyjä kysymyksiä in-place eDiscovery- ja in-Place Holds -laatoista](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



