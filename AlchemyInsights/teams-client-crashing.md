---
title: Teams ohjelma kaatuu
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
ms.openlocfilehash: a292e160abcfc26ffebc454d32ee489a319a23f4bb81e70fe5dbe72bfd0b8b81
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890335"
---
# <a name="teams-client-crashing"></a>Teams ohjelma kaatuu

Jos Teams-ohjelmasi kaatuu, kokeile seuraavia keinoja:

- Jos käytät Teams-työpöytäsovellusta, varmista, että [sovellus on täysin ajan tasalla](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Varmista, että kaikki [Microsoft 365:n URL-osoitteet ja osoitealueet](https://docs.microsoft.com/microsoftteams/connectivity-issues) ovat käytettävissä.

- Kirjaudu sisään vuokraajan järjestelmänvalvojatilillä ja tarkista [Palvelun kunnon koontinäytöstä](https://docs.microsoft.com/office365/enterprise/view-service-health), että palvelussa ei ole käyttökatkoja tai rajoituksia.

- Poista Teams-sovellus ja asenna se uudelleen
    - Siirry tietokoneen %appdata%\Microsoft\Teams\-kansioon ja poista kaikki hakemiston tiedostot.
    - [Lataa ja asenna Teams -sovellus](https://www.microsoft.com/microsoft-teams/download-app)ja asenna Teams järjestelmänvalvojana (napsauta Teams-asennusohjelmaa hiiren kakkospainikkeella ja valitse Suorita **järjestelmänvalvojana,** jos saatavilla).

Jos Teams edelleen kaatuu, yritä kopioida ongelma uudelleen. Jos voit:

1. Käytä vaiheiden tallenninta vaiheiden tallentamiseen.
    - Sulje KAIKKI tarpeettomat tai luottamukselliset sovellukset.
    - Käynnistä vaiheiden tallennin ja toista ongelma kirjautuneena sisään sillä käyttäjätilillä, jota ongelma koskee.
    - [Kerää teams-lokit, jotka kirjaavat tallennetut toistetut vaiheet](https://docs.microsoft.com/microsoftteams/log-files). **Huomautus**: Varmista, että otat kuvan sen käyttäjän kirjautumisosoitteen, jota ongelma koskee.
    - Kerää varmuuskopion ja/tai vikasäiliön tiedot (Windows). Käynnistä Windows Powershell siinä koneessa, jossa kaatuminen tapahtuu, ja suorita seuraavat komennot (paina jokaisen komennon jälkeen Enter-näppäintä):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Kun tekstitiedosto on luotu ja se tulee näyttöön, tallenna tiedosto ja liitä se palvelupyyntöön. 
