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
# <a name="teams-client-crashing"></a><span data-ttu-id="9b297-102">Kaatuuko Teams?</span><span class="sxs-lookup"><span data-stu-id="9b297-102">Teams client crashing?</span></span>

<span data-ttu-id="9b297-103">Jos Teams-ohjelmasi kaatuu, kokeile seuraavia keinoja:</span><span class="sxs-lookup"><span data-stu-id="9b297-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="9b297-104">Jos käytät Teams-työpöytäsovellusta, varmista, että [sovellus on täysin ajan tasalla](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="9b297-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="9b297-105">Varmista, että kaikki [Microsoft 365:n URL-osoitteet ja osoitealueet](https://docs.microsoft.com/microsoftteams/connectivity-issues) ovat käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="9b297-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="9b297-106">Kirjaudu sisään vuokraajan järjestelmänvalvojan tilillä ja tarkista [Palvelun kunnon hallintapaneelista,](https://docs.microsoft.com/office365/enterprise/view-service-health) ettei käyttökatkoja tai palvelun heikkenemistä ole.</span><span class="sxs-lookup"><span data-stu-id="9b297-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="9b297-107">Teams-sovelluksen asennuksen poistaminen ja asentaminen uudelleen (linkki)</span><span class="sxs-lookup"><span data-stu-id="9b297-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="9b297-108">Siirry tietokoneen %appdata%\Microsoft\teams\-kansioon ja poista kaikki kyseisen kansion tiedostot.</span><span class="sxs-lookup"><span data-stu-id="9b297-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="9b297-109">[Lataa ja asenna Teams-sovellus](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)ja asenna Teams järjestelmänvalvojana (napsauta teams-asennusohjelmaa hiiren kakkospainikkeella ja valitse Suorita järjestelmänvalvojana, jos sellainen on).</span><span class="sxs-lookup"><span data-stu-id="9b297-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="9b297-110">Jos Teams-asiakkaasi kaatuu edelleen, voitko toistaa ongelman?</span><span class="sxs-lookup"><span data-stu-id="9b297-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="9b297-111">Jos näin on:</span><span class="sxs-lookup"><span data-stu-id="9b297-111">If so:</span></span>

1. <span data-ttu-id="9b297-112">Ota askeleet vaiheiden avulla.</span><span class="sxs-lookup"><span data-stu-id="9b297-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="9b297-113">Sulje kaikki tarpeettomat tai luottamukselliset sovellukset.</span><span class="sxs-lookup"><span data-stu-id="9b297-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="9b297-114">Käynnistä Steps Recorder ja toista ongelma, kun olet kirjautunut sisään haavoittuvuuden sisältävällä käyttäjätilillä.</span><span class="sxs-lookup"><span data-stu-id="9b297-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="9b297-115">[Kerää joukkueet lokit, jotka kaapata kirjataan repro vaiheet](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="9b297-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="9b297-116">**Huomautus**: Varmista, että sieppaat vaikutusalueen vaikuttaneen käyttäjän kirjautumisosoitteen.</span><span class="sxs-lookup"><span data-stu-id="9b297-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="9b297-117">Kerää vedos- ja/tai vikasäilön tiedot (Windows).</span><span class="sxs-lookup"><span data-stu-id="9b297-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="9b297-118">Käynnistä Windows Powershell tietokoneessa, jossa kaatuminen tapahtuu, ja suorita seuraavat komennot:</span><span class="sxs-lookup"><span data-stu-id="9b297-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="9b297-119">Liitä tiedosto tukikoteloosi.</span><span class="sxs-lookup"><span data-stu-id="9b297-119">Attach the file to your support case.</span></span>
