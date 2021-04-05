---
title: Levytilan vapauttaminen Windows 10:ssä
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
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505353"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="ae044-102">Levytilan vapauttaminen Windows 10:ssä</span><span class="sxs-lookup"><span data-stu-id="ae044-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="ae044-103">Tässä on kaksi vaihtoehtoa levytilan vapauttamiseen Windowsissa:</span><span class="sxs-lookup"><span data-stu-id="ae044-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="ae044-104">Levytilan vapauttaminen Windows 10:ssä.</span><span class="sxs-lookup"><span data-stu-id="ae044-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="ae044-105">Levytilan vapauttaminen Windows 10 -päivityksille ulkoisella tallennuslaitteella.</span><span class="sxs-lookup"><span data-stu-id="ae044-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="ae044-106">Jos sinulla on yhä vähän levytilaa levyn uudelleenjärjestämisen jälkeen, Temp-kansiosi saattaa mahdollisesti täyttyä nopeasti Microsoft Storen käyttämillä sovellustiedostoilla (.appx).</span><span class="sxs-lookup"><span data-stu-id="ae044-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="ae044-107">Voit korjata ongelman palauttamalla Storen, tyhjentämällä Storen välimuistin ja suorittamalla sitten Windows Updaten vianmäärityksen.</span><span class="sxs-lookup"><span data-stu-id="ae044-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="ae044-108">Varmista, että Microsoft Store on suljettu, ennen kuin käytät näitä vaiheita.</span><span class="sxs-lookup"><span data-stu-id="ae044-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="ae044-109">**Vaihe 1: Palauta Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="ae044-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="ae044-110">**Huomautus** Tämä poistaa pysyvästi sovellustiedot laitteesta, mukaan lukien asetukset ja kirjautumistiedot.</span><span class="sxs-lookup"><span data-stu-id="ae044-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="ae044-111">Valitse **Aloitus** > **Asetukset** > **Sovellukset** > **Sovellukset ja ominaisuudet**.</span><span class="sxs-lookup"><span data-stu-id="ae044-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="ae044-112">Etsi ja valitse sovellusluettelosta Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="ae044-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="ae044-113">Valitse **Lisäasetukset**.</span><span class="sxs-lookup"><span data-stu-id="ae044-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="ae044-114">Vieritä alaspäin ja valitse **Palauta**, ja valitse sitten **Vahvista palautus**.</span><span class="sxs-lookup"><span data-stu-id="ae044-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="ae044-115">**Vaihe 2: Microsoft Storen välimuistin tyhjentäminen**</span><span class="sxs-lookup"><span data-stu-id="ae044-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="ae044-116">Avaa Suorita-valintaikkuna painamalla näppäinyhdistelmää Windows-näppäin + R.</span><span class="sxs-lookup"><span data-stu-id="ae044-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="ae044-117">Kirjoita wsreset.exe ja valitse **OK**.</span><span class="sxs-lookup"><span data-stu-id="ae044-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="ae044-118">Tyhjä komentokehoteikkuna avautuu.</span><span class="sxs-lookup"><span data-stu-id="ae044-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="ae044-119">Noin 10 sekunnin kuluttua ikkuna sulkeutuu, ja Store avautuu automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="ae044-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="ae044-120">**Vaihe 3: Palauta Windows Update**</span><span class="sxs-lookup"><span data-stu-id="ae044-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="ae044-121">Valitse **Aloitus** > **Asetukset** > **Päivittäminen ja suojaus** > **Vianmääritys**.</span><span class="sxs-lookup"><span data-stu-id="ae044-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="ae044-122">Vieritä alaspäin ja valitse luettelosta **Windows Update**, ja valitse **Suorita vianmääritys**.</span><span class="sxs-lookup"><span data-stu-id="ae044-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="ae044-123">Käynnistä tietokone uudelleen ja tarkista, ilmeneekö ongelma edelleen.</span><span class="sxs-lookup"><span data-stu-id="ae044-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

