---
title: Kaatuuko Teams?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354049"
---
# <a name="teams-client-crashing"></a>Kaatuuko Teams?

Jos Teams-ohjelmasi kaatuu, kokeile seuraavia keinoja:

- Jos käytät Teams-työpöytäsovellusta, varmista, että [sovellus on täysin ajan tasalla](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Varmista, että kaikki [Microsoft 365:n URL-osoitteet ja osoitealueet](https://docs.microsoft.com/microsoftteams/connectivity-issues) ovat käytettävissä.

- Kirjaudu sisään vuokraajan järjestelmänvalvojan tilillä ja tarkista [Palvelun kunnon hallintapaneelista,](https://docs.microsoft.com/office365/enterprise/view-service-health) ettei käyttökatkoja tai palvelun heikkenemistä ole.

- Teams-sovelluksen asennuksen poistaminen ja asentaminen uudelleen (linkki)
    - Siirry tietokoneen %appdata%\Microsoft\teams\-kansioon ja poista kaikki kyseisen kansion tiedostot.
    - [Lataa ja asenna Teams-sovellus](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)ja asenna Teams järjestelmänvalvojana (napsauta teams-asennusohjelmaa hiiren kakkospainikkeella ja valitse Suorita järjestelmänvalvojana, jos sellainen on).

Jos Teams-asiakkaasi kaatuu edelleen, voitko toistaa ongelman? Jos näin on:

1. Ota askeleet vaiheiden avulla.
    - Sulje kaikki tarpeettomat tai luottamukselliset sovellukset.
    - Käynnistä Steps Recorder ja toista ongelma, kun olet kirjautunut sisään haavoittuvuuden sisältävällä käyttäjätilillä.
    - [Kerää joukkueet lokit, jotka kaapata kirjataan repro vaiheet](https://docs.microsoft.com/microsoftteams/log-files). **Huomautus**: Varmista, että sieppaat vaikutusalueen vaikuttaneen käyttäjän kirjautumisosoitteen.
    - Kerää vedos- ja/tai vikasäilön tiedot (Windows). Käynnistä Windows Powershell tietokoneessa, jossa kaatuminen tapahtuu, ja suorita seuraavat komennot:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Liitä tiedosto tukikoteloosi.
