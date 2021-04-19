---
title: Windowsin muistin diagnostiikan käyttö Windows 10:ssä
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
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826664"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="3f42b-102">Windowsin muistin diagnostiikan käyttö Windows 10:ssä</span><span class="sxs-lookup"><span data-stu-id="3f42b-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="3f42b-103">Jos tietokoneesi Windows ja sovellukset kaatavat, jäädyvät tai toimivat epävakaalla tavalla, tietokoneen muistissa (RAM-muistissa) voi olla ongelma.</span><span class="sxs-lookup"><span data-stu-id="3f42b-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="3f42b-104">Voit tarkistaa tietokoneen RAM-muistiongelmat Windowsin muistin diagnostiikan avulla.</span><span class="sxs-lookup"><span data-stu-id="3f42b-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="3f42b-105">Kirjoita tehtäväpalkin hakuruutuun muistin **vianmääritys** ja valitse sitten **Windowsin muistin vianmääritys**.</span><span class="sxs-lookup"><span data-stu-id="3f42b-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="3f42b-106">Jotta voit suorittaa vianmäärityksen, tietokone on käynnistettävä uudelleen.</span><span class="sxs-lookup"><span data-stu-id="3f42b-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="3f42b-107">Voit käynnistää vianmäärityksen heti uudelleen (tallenna työsi ja sulje ensin avoimet asiakirjat ja sähköpostiviestit) tai ajoita vianmääritys toimimaan automaattisesti, kun tietokone seuraavan kerran käynnistyy uudelleen:</span><span class="sxs-lookup"><span data-stu-id="3f42b-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windowsin muistin vianmääritys](media/windows-memory-diagnostic.png)

<span data-ttu-id="3f42b-109">Kun tietokone käynnistyy uudelleen, **Windowsin muistin diagnostiikkatyökalu** toimii automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="3f42b-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="3f42b-110">Tila ja edistyminen näytetään diagnostiikan suorittamisen aikana, ja voit peruuttaa diagnostiikan  painamalla ESC-näppäintä.</span><span class="sxs-lookup"><span data-stu-id="3f42b-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="3f42b-111">Kun diagnostiikka on valmis, Windows käynnistyy normaalisti.</span><span class="sxs-lookup"><span data-stu-id="3f42b-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="3f42b-112">Heti uudelleenkäynnistyksen jälkeen näyttöön tulee työpöytä-ilmoitus (tehtäväpalkin Toimintokeskus-kuvakkeen vieressä) sen merkiksi, löytyikö muistivirheitä. </span><span class="sxs-lookup"><span data-stu-id="3f42b-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="3f42b-113">Esimerkkejä:</span><span class="sxs-lookup"><span data-stu-id="3f42b-113">For example:</span></span>

<span data-ttu-id="3f42b-114">Tässä on Toimintokeskus-kuvake:</span><span class="sxs-lookup"><span data-stu-id="3f42b-114">Here's the Action Center icon:</span></span> ![Toimintokeskuksen kuvake](media/action-center-icon.png) 

<span data-ttu-id="3f42b-116">Esimerkkiilmoitus:</span><span class="sxs-lookup"><span data-stu-id="3f42b-116">And a sample notification:</span></span> ![Ei muistivirheitä](media/no-memory-errors.png)

<span data-ttu-id="3f42b-118">Jos et saanut ilmoitusta, voit  tuoda toimintokeskuksen näkyviin ja  tarkastella vieritettävää ilmoitusluetteloa valitsemalla tehtäväpalkista Toimintokeskus-kuvakkeen.</span><span class="sxs-lookup"><span data-stu-id="3f42b-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="3f42b-119">Voit tarkastella yksityiskohtaisia tietoja **kirjoittamalla tapahtuman** tehtäväpalkin hakuruutuun ja valitsemalla sitten **Tapahtumienvalvonta**.</span><span class="sxs-lookup"><span data-stu-id="3f42b-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="3f42b-120">Siirry **Tapahtumienvalvonnan** vasemmanpuoleisessa ruudussa kohtaan **Windows-lokit > järjestelmä**.</span><span class="sxs-lookup"><span data-stu-id="3f42b-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="3f42b-121">Etsi oikeanpuoleisessa ruudussa luetteloa samalla,  kun tarkastelet Lähde-saraketta, kunnes näet Tapahtumat, joiden arvo on **Lähdearvo MemoryDiagnostics-Results.**</span><span class="sxs-lookup"><span data-stu-id="3f42b-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="3f42b-122">Korosta kukin tapahtuma ja katso tulostiedot luettelon alapuolella olevassa **Yleiset-välilehden** ruudussa.</span><span class="sxs-lookup"><span data-stu-id="3f42b-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
