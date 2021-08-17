---
title: Vanhojen eDiscovery-työkalujen käytöstä poisto
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
- "9001487"
- "3523"
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074671"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Vanhojen eDiscovery-työkalujen käytöstä poisto

Microsoft 365 -yhteensopivuuskeskuksen uusien ja parannettujen eDiscovery-toimintojen ansiosta seuraavat vanhat eDiscovery-työkalut ja -komentojen komennot eivät enää ole käytettävissä seuraavien kuukausien aikana:

- [Aseta eDiscovery-pito](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [ja pito](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Exchange hallintakeskuksessa.

- PowerShellin Exchange Online cmdlet-komennot, jotka In-Place eDiscovery- ja In-Place-pitoa. (Nämä cmdlet-komennot tunnistetaan yhteisesti *-MailboxSearch-cmdlet-komennoiksi.) Tämä sisältää seuraavat cmdlet-komennot:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [PowerShellin](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) Search-Mailbox-cmdlet-Exchange Online.
- Seuraavat toiminnot Web Services -Exchange ohjelmointirajapinnassa:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Aikajana käytöstä poistolle:**
- **1. heinäkuuta 2020** Et voi enää luoda uusia hakuja ja pitoja, mutta voit suorittaa, muokata ja poistaa aiemmin luotuja hakuja omalla vastuullasi. Microsoft-tuki ei enää In-Place eDiscovery& pitoa EAC:ssä.
    
- **1. lokakuuta 2020** In-Place eDiscovery & EAC:n Pitotoiminnot sijoitetaan vain luku -tilaan, joten voit poistaa vain aiemmin luodut haut ja pitotoiminnot.

**Lisätietoja on kohdassa:**

 - [Vanhojen eDiscovery-hakujen ja -pitojen siirtäminen Microsoft 365 -yhteensopivuuskeskus](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Vanhojen eDiscovery-työkalujen käytöstä poisto](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Usein kysyttyjä kysymyksiä eDiscoveryIn-Place ja In-Place pitoon liittyen](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



