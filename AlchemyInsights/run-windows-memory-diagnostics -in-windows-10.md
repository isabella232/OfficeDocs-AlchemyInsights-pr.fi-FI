---
title: Windowsin muistin diagnostiikan suorittaminen Windows 10:ssä
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357514"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="97f72-102">Windowsin muistin diagnostiikan suorittaminen Windows 10:ssä</span><span class="sxs-lookup"><span data-stu-id="97f72-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="97f72-103">Jos tietokoneen Windows ja sovellukset kaatuvat, jäädyttävät tai toimivat epävakaalla tavalla, tietokoneen muistissa (RAM) saattaa olla ongelma.</span><span class="sxs-lookup"><span data-stu-id="97f72-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="97f72-104">Voit tarkistaa tietokoneen RAM-muistin ongelmat suorittamalla Windowsin muistin diagnostiikan.</span><span class="sxs-lookup"><span data-stu-id="97f72-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="97f72-105">Kirjoita tehtäväpalkin hakuruutuun **muistin diagnostiikka**ja valitse sitten **Windowsin muistin diagnostiikka**.</span><span class="sxs-lookup"><span data-stu-id="97f72-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="97f72-106">Jotta voit suorittaa vianmäärityksen, tietokoneen on käynnistettävä uudelleen.</span><span class="sxs-lookup"><span data-stu-id="97f72-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="97f72-107">Voit käynnistää tietokoneen uudelleen välittömästi (tallenna työsi ja sulje ensin avoimet asiakirjat ja sähköpostiviestit) tai ajoittaa diagnostiikan käynnistymään automaattisesti, kun tietokone käynnistetään seuraavan kerran uudelleen:</span><span class="sxs-lookup"><span data-stu-id="97f72-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windowsin muistin diagnostiikka](media/windows-memory-diagnostic.png)

<span data-ttu-id="97f72-109">Kun tietokone käynnistyy uudelleen, **Windowsin muistin diagnostiikkatyökalu** käynnistyy automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="97f72-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="97f72-110">Tila ja edistyminen näytetään diagnostiikan suorittamisen ajona, ja voit peruuttaa diagnostiikan painamalla näppäimistön **ESC-näppäintä.**</span><span class="sxs-lookup"><span data-stu-id="97f72-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="97f72-111">Kun diagnostiikka on valmis, Windows käynnistyy normaalisti.</span><span class="sxs-lookup"><span data-stu-id="97f72-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="97f72-112">Heti uudelleenkäynnistyksen jälkeen, kun työpöytä tulee näkyviin, **Action Center** näyttöön tulee ilmoitus (tehtäväpalkin Toimintokeskus-kuvakkeen vieressä), joka ilmaisee, onko muistivirheitä löytynyt.</span><span class="sxs-lookup"><span data-stu-id="97f72-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="97f72-113">Esimerkiksi:</span><span class="sxs-lookup"><span data-stu-id="97f72-113">For example:</span></span>

<span data-ttu-id="97f72-114">Tässä on Toimintokeskus-kuvake:</span><span class="sxs-lookup"><span data-stu-id="97f72-114">Here's the Action Center icon:</span></span> ![Toimintokeskuksen kuvake](media/action-center-icon.png) 

<span data-ttu-id="97f72-116">Ja näyte ilmoitus:</span><span class="sxs-lookup"><span data-stu-id="97f72-116">And a sample notification:</span></span> ![Ei muistivirheitä](media/no-memory-errors.png)

<span data-ttu-id="97f72-118">Jos et huomannut ilmoitusta, voit tuoda **toimintokeskuksen** näkyviin valitsemalla tehtäväpalkin **Toimintokeskus-kuvakkeen** ja nähdä vieritettävän ilmoitusluettelon.</span><span class="sxs-lookup"><span data-stu-id="97f72-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="97f72-119">Voit tarkastella yksityiskohtaisia tietoja kirjoittamalla **tehtäväpalkin** hakuruutuun tapahtuman ja valitsemalla sitten **Tapahtumienvalvonta**.</span><span class="sxs-lookup"><span data-stu-id="97f72-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="97f72-120">Siirry **Tapahtumienvalvonnan**vasemmanpuoleisessa ruudussa **Windowsin lokit-> järjestelmä**.</span><span class="sxs-lookup"><span data-stu-id="97f72-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="97f72-121">Skannaa oikeanpuoleisessa ruudussa luettelo alaspäin, kun tarkastelet **Lähde-saraketta,** kunnes näet tapahtumat, joiden **Lähde-arvo on MemoryDiagnostics-Results**.</span><span class="sxs-lookup"><span data-stu-id="97f72-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="97f72-122">Korosta jokainen tällainen tapahtuma ja katso tulostiedot luettelon alapuolella olevan **Yleiset-välilehden** alla olevasta ruudusta.</span><span class="sxs-lookup"><span data-stu-id="97f72-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
