---
title: Levytilan säästäminen Windows 10:ssä
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036592"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="0196e-102">Levytilan säästäminen Windows 10:ssä</span><span class="sxs-lookup"><span data-stu-id="0196e-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="0196e-103">Voit vapauttaa levytilaa Windowsissa kahdella eri vaihtoehdolla:</span><span class="sxs-lookup"><span data-stu-id="0196e-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="0196e-104">Vapauttaa levytilaa Windows 10:ssä.</span><span class="sxs-lookup"><span data-stu-id="0196e-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="0196e-105">Voit vapauttaa tilaa Windows 10:n päivityksille ulkoisella tallennuslaitteella.</span><span class="sxs-lookup"><span data-stu-id="0196e-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="0196e-106">Jos levytila on edelleen vähissä levyn uudelleenjärjestämisen käytön jälkeen, tilapäiskansio voi täyttää nopeasti Microsoft Storen käyttämät sovellustiedostot (.appx).</span><span class="sxs-lookup"><span data-stu-id="0196e-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="0196e-107">Voit korjata ongelman palauttamalla Kaupan oletusasetukset, tyhjentää Kaupan välimuistin ja suorittaa sitten Windows Updaten vianmäärityksen.</span><span class="sxs-lookup"><span data-stu-id="0196e-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="0196e-108">Varmista, että Microsoft Store on suljettu, ennen kuin jatkat näillä ohjeilla.</span><span class="sxs-lookup"><span data-stu-id="0196e-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="0196e-109">**Vaihe 1: Palauta Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="0196e-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="0196e-110">**Huomautus** Tämä poistaa sovelluksen tiedot pysyvästi laitteesta, mukaan lukien mieltymyksesi ja kirjautumistietosi.</span><span class="sxs-lookup"><span data-stu-id="0196e-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="0196e-111">Valitse   >  **Aloitusasetukset-sovellussovellukset**  >    >  **& ominaisuudet.**</span><span class="sxs-lookup"><span data-stu-id="0196e-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="0196e-112">Etsi ja valitse sovellusluettelosta Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="0196e-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="0196e-113">Valitse **Lisäasetukset.**</span><span class="sxs-lookup"><span data-stu-id="0196e-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="0196e-114">Vieritä alaspäin, **valitse Palauta** ja vahvista **palautus.**</span><span class="sxs-lookup"><span data-stu-id="0196e-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="0196e-115">**Vaihe 2: Microsoft Storen välimuistin tyhjentäminen**</span><span class="sxs-lookup"><span data-stu-id="0196e-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="0196e-116">Avaa Suorita-valintaikkuna painamalla näppäinyhdistelmää Windows-näppäin + R.</span><span class="sxs-lookup"><span data-stu-id="0196e-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="0196e-117">Kirjoita wsreset.exe ja valitse **OK.**</span><span class="sxs-lookup"><span data-stu-id="0196e-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="0196e-118">Näyttöön avautuu tyhjä komentokehoteikkuna.</span><span class="sxs-lookup"><span data-stu-id="0196e-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="0196e-119">Noin 10 sekunnin kuluttua ikkuna sulkeutuu ja Kauppa avautuu automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="0196e-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="0196e-120">**Vaihe 3: Palauta Windows Update**</span><span class="sxs-lookup"><span data-stu-id="0196e-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="0196e-121">Valitse **Start**  >  **Settings**  >  **Update & Security**  >  **Troubleshoot**.</span><span class="sxs-lookup"><span data-stu-id="0196e-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="0196e-122">Vieritä alaspäin, **valitse Windows Update** luettelosta ja valitse Suorita **vianmääritys.**</span><span class="sxs-lookup"><span data-stu-id="0196e-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="0196e-123">Käynnistä tietokone uudelleen ja tarkista, onko ongelma yhä ongelmassa.</span><span class="sxs-lookup"><span data-stu-id="0196e-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

