---
title: Kaatuuko Teams?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826268"
---
# <a name="teams-client-crashing"></a>Kaatuuko Teams?

Jos Teams-ohjelmasi kaatuu, kokeile seuraavia keinoja:

- Jos käytät Teams-työpöytäsovellusta, varmista, että [sovellus on täysin ajan tasalla](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Varmista, että kaikki [Microsoft 365:n URL-osoitteet ja osoitealueet](https://docs.microsoft.com/microsoftteams/connectivity-issues) ovat käytettävissä.

- Kirjaudu sisään vuokraajan järjestelmänvalvojatilillä ja tarkista [Palvelun kunnon koontinäytöstä](https://docs.microsoft.com/office365/enterprise/view-service-health), että palvelussa ei ole käyttökatkoja tai rajoituksia.

- Teams-sovelluksen asennuksen poistaminen ja uudelleenasentaminen (linkki)
    - Siirry tietokoneen %appdata%\Microsoft\teams\-kansioon ja poista kaikki tämän hakemiston tiedostot.
    - [Lataa ja asenna Teams-sovellus](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), ja jos mahdollista, asenna Teams järjestelmänvalvojana (napsauta Teams-asennusohjelmaa hiiren kakkospainikkeella ja valitse Suorita järjestelmänvalvojana, jos saatavilla).

Jos Teams-asiakasohjelmasi kaatuu edelleen, voitko toistaa ongelman? Jos näin on:

1. Käytä vaiheiden tallenninta vaiheiden tallentamiseen.
    - Sulje KAIKKI tarpeettomat tai luottamukselliset sovellukset.
    - Käynnistä vaiheiden tallennin ja toista ongelma kirjautuneena sisään sillä käyttäjätilillä, jota ongelma koskee.
    - [Kerää teams-lokit, jotka kirjaavat tallennetut toistetut vaiheet](https://docs.microsoft.com/microsoftteams/log-files). **Huomautus**: Varmista, että otat kuvan sen käyttäjän kirjautumisosoitteen, jota ongelma koskee.
    - Kerää varmuuskopion ja/tai vikasäiliön tiedot (Windows). Käynnistä Windows PowerShell siinä koneessa, jossa kaatuminen ilmenee, ja suorita seuraavat komennot:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Liitä tiedosto tukitapaukseen.
