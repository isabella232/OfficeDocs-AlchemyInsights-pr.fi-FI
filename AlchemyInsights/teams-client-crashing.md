---
title: Teams-asiakasohjelma kaatuu
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187718"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="fd23d-102">Teams-asiakasohjelma kaatuu</span><span class="sxs-lookup"><span data-stu-id="fd23d-102">Teams client crashing</span></span>

<span data-ttu-id="fd23d-103">Jos Teams-ohjelmasi kaatuu, kokeile seuraavia keinoja:</span><span class="sxs-lookup"><span data-stu-id="fd23d-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="fd23d-104">Jos käytät Teams-työpöytäsovellusta, varmista, että [sovellus on täysin ajan tasalla](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="fd23d-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="fd23d-105">Varmista, että kaikki [Microsoft 365:n URL-osoitteet ja osoitealueet](/microsoftteams/connectivity-issues) ovat käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="fd23d-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="fd23d-106">Kirjaudu sisään vuokraajan järjestelmänvalvojatilillä ja tarkista [Palvelun kunnon koontinäytöstä](/office365/enterprise/view-service-health), että palvelussa ei ole käyttökatkoja tai rajoituksia.</span><span class="sxs-lookup"><span data-stu-id="fd23d-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="fd23d-107">Poista Teams-sovellus ja asenna se uudelleen</span><span class="sxs-lookup"><span data-stu-id="fd23d-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="fd23d-108">Siirry tietokoneen %appdata%\Microsoft\Teams\-kansioon ja poista kaikki hakemiston tiedostot.</span><span class="sxs-lookup"><span data-stu-id="fd23d-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="fd23d-109">[Lataa ja asenna Teams -sovellus](https://www.microsoft.com/microsoft-teams/download-app)ja asenna Teams järjestelmänvalvojana (napsauta Teams-asennusohjelmaa hiiren kakkospainikkeella ja valitse **Suorita** järjestelmänvalvojana, jos saatavilla).</span><span class="sxs-lookup"><span data-stu-id="fd23d-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="fd23d-110">Jos Teams edelleen kaatuu, yritä kopioida ongelma uudelleen.</span><span class="sxs-lookup"><span data-stu-id="fd23d-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="fd23d-111">Jos voit:</span><span class="sxs-lookup"><span data-stu-id="fd23d-111">If you can:</span></span>

1. <span data-ttu-id="fd23d-112">Käytä vaiheiden tallenninta vaiheiden tallentamiseen.</span><span class="sxs-lookup"><span data-stu-id="fd23d-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="fd23d-113">Sulje KAIKKI tarpeettomat tai luottamukselliset sovellukset.</span><span class="sxs-lookup"><span data-stu-id="fd23d-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="fd23d-114">Käynnistä vaiheiden tallennin ja toista ongelma kirjautuneena sisään sillä käyttäjätilillä, jota ongelma koskee.</span><span class="sxs-lookup"><span data-stu-id="fd23d-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="fd23d-115">[Kerää teams-lokit, jotka kirjaavat tallennetut toistetut vaiheet](/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="fd23d-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="fd23d-116">**Huomautus**: Varmista, että otat kuvan sen käyttäjän kirjautumisosoitteen, jota ongelma koskee.</span><span class="sxs-lookup"><span data-stu-id="fd23d-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="fd23d-117">Kerää varmuuskopion ja/tai vikasäiliön tiedot (Windows).</span><span class="sxs-lookup"><span data-stu-id="fd23d-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="fd23d-118">Käynnistä Windows Powershell siinä koneessa, jossa kaatuminen tapahtuu, ja suorita seuraavat komennot (paina jokaisen komennon jälkeen Enter-näppäintä):</span><span class="sxs-lookup"><span data-stu-id="fd23d-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="fd23d-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="fd23d-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="fd23d-120">Kun tekstitiedosto on luotu ja se tulee näyttöön, tallenna tiedosto ja liitä se palvelupyyntöön.</span><span class="sxs-lookup"><span data-stu-id="fd23d-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
