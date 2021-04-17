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
# <a name="teams-client-crashing"></a><span data-ttu-id="23ed5-102">Kaatuuko Teams?</span><span class="sxs-lookup"><span data-stu-id="23ed5-102">Teams client crashing?</span></span>

<span data-ttu-id="23ed5-103">Jos Teams-ohjelmasi kaatuu, kokeile seuraavia keinoja:</span><span class="sxs-lookup"><span data-stu-id="23ed5-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="23ed5-104">Jos käytät Teams-työpöytäsovellusta, varmista, että [sovellus on täysin ajan tasalla](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="23ed5-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="23ed5-105">Varmista, että kaikki [Microsoft 365:n URL-osoitteet ja osoitealueet](https://docs.microsoft.com/microsoftteams/connectivity-issues) ovat käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="23ed5-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="23ed5-106">Kirjaudu sisään vuokraajan järjestelmänvalvojatilillä ja tarkista [Palvelun kunnon koontinäytöstä](https://docs.microsoft.com/office365/enterprise/view-service-health), että palvelussa ei ole käyttökatkoja tai rajoituksia.</span><span class="sxs-lookup"><span data-stu-id="23ed5-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="23ed5-107">Teams-sovelluksen asennuksen poistaminen ja uudelleenasentaminen (linkki)</span><span class="sxs-lookup"><span data-stu-id="23ed5-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="23ed5-108">Siirry tietokoneen %appdata%\Microsoft\teams\-kansioon ja poista kaikki tämän hakemiston tiedostot.</span><span class="sxs-lookup"><span data-stu-id="23ed5-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="23ed5-109">[Lataa ja asenna Teams-sovellus](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), ja jos mahdollista, asenna Teams järjestelmänvalvojana (napsauta Teams-asennusohjelmaa hiiren kakkospainikkeella ja valitse Suorita järjestelmänvalvojana, jos saatavilla).</span><span class="sxs-lookup"><span data-stu-id="23ed5-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="23ed5-110">Jos Teams-asiakasohjelmasi kaatuu edelleen, voitko toistaa ongelman?</span><span class="sxs-lookup"><span data-stu-id="23ed5-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="23ed5-111">Jos näin on:</span><span class="sxs-lookup"><span data-stu-id="23ed5-111">If so:</span></span>

1. <span data-ttu-id="23ed5-112">Käytä vaiheiden tallenninta vaiheiden tallentamiseen.</span><span class="sxs-lookup"><span data-stu-id="23ed5-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="23ed5-113">Sulje KAIKKI tarpeettomat tai luottamukselliset sovellukset.</span><span class="sxs-lookup"><span data-stu-id="23ed5-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="23ed5-114">Käynnistä vaiheiden tallennin ja toista ongelma kirjautuneena sisään sillä käyttäjätilillä, jota ongelma koskee.</span><span class="sxs-lookup"><span data-stu-id="23ed5-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="23ed5-115">[Kerää teams-lokit, jotka kirjaavat tallennetut toistetut vaiheet](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="23ed5-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="23ed5-116">**Huomautus**: Varmista, että otat kuvan sen käyttäjän kirjautumisosoitteen, jota ongelma koskee.</span><span class="sxs-lookup"><span data-stu-id="23ed5-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="23ed5-117">Kerää varmuuskopion ja/tai vikasäiliön tiedot (Windows).</span><span class="sxs-lookup"><span data-stu-id="23ed5-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="23ed5-118">Käynnistä Windows PowerShell siinä koneessa, jossa kaatuminen ilmenee, ja suorita seuraavat komennot:</span><span class="sxs-lookup"><span data-stu-id="23ed5-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="23ed5-119">Liitä tiedosto tukitapaukseen.</span><span class="sxs-lookup"><span data-stu-id="23ed5-119">Attach the file to your support case.</span></span>
