---
title: Käynnistysasetukset Windows 10:ssä
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828149"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="02bac-102">Käynnistysasetukset Windows 10:ssä</span><span class="sxs-lookup"><span data-stu-id="02bac-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="02bac-103">**Muuta, mitkä sovellukset suoritetaan automaattisesti käynnistyksen yhteydessä**</span><span class="sxs-lookup"><span data-stu-id="02bac-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="02bac-104">Valitse Asetukset [> sovellukset > käynnistys .](ms-settings:startupapps?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="02bac-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="02bac-105">Varmista, että mikä tahansa käynnistettäessä suoritettava sovellus **on** käytössä .</span><span class="sxs-lookup"><span data-stu-id="02bac-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="02bac-106">**Sovelluksen lisääminen automaattisesti suoritettavaksi käynnistyksen yhteydessä**</span><span class="sxs-lookup"><span data-stu-id="02bac-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="02bac-107">Valitse Käynnistä **ja** etsi sovellus, jonka haluat suorittaa käynnistyksen yhteydessä.</span><span class="sxs-lookup"><span data-stu-id="02bac-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="02bac-108">Napsauta sovellusta hiiren kakkospainikkeella, **valitse Lisää** ja valitse sitten **Avaa tiedostosijainti**.</span><span class="sxs-lookup"><span data-stu-id="02bac-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="02bac-109">Tämä avaa sijainnin, johon sovelluksen pikakuvake on tallennettu.</span><span class="sxs-lookup"><span data-stu-id="02bac-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="02bac-110">Jos Avaa tiedostosijainti -vaihtoehtoa ei ole, sovellusta ei voi suorittaa käynnistyksen yhteydessä.</span><span class="sxs-lookup"><span data-stu-id="02bac-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="02bac-111">Kun tiedostosijainti on auki, paina **näppäinyhdistelmää Windows-näppäin + R,** **kirjoita shell:startup** ja valitse **sitten OK**.</span><span class="sxs-lookup"><span data-stu-id="02bac-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="02bac-112">Tämä avaa Käynnistys-kansion.</span><span class="sxs-lookup"><span data-stu-id="02bac-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="02bac-113">Kopioi ja liitä pikakuvake sovellukseen tiedoston sijainnista Käynnistys-kansioon.</span><span class="sxs-lookup"><span data-stu-id="02bac-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="02bac-114">**Käynnistyksen lisäasetukset (mukaan lukien vikasietotila, UEFI-asetukset ja käynnistys toisesta laitteesta)**</span><span class="sxs-lookup"><span data-stu-id="02bac-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="02bac-115">Tallenna työsi ja sulje kaikki avoimet tiedostot, koska nämä vaiheet käynnistävät tietokoneen uudelleen.</span><span class="sxs-lookup"><span data-stu-id="02bac-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="02bac-116">Siirry kohtaan [Asetukset > päivittäminen & suojausasetusten > palautus.](ms-settings:recovery?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="02bac-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="02bac-117">Valitse **Käynnistyksen lisäasetukset**-kohdassa **Käynnistä uudelleen nyt**.</span><span class="sxs-lookup"><span data-stu-id="02bac-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="02bac-118">Kun tietokone käynnistyy uudelleen Valitse vaihtoehto -näyttöön:</span><span class="sxs-lookup"><span data-stu-id="02bac-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="02bac-119">Jos haluat käynnistää laitteen, kuten USB-muistitikun, valitse **Käytä laitetta**.</span><span class="sxs-lookup"><span data-stu-id="02bac-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="02bac-120">Jos haluat määrittää UEFI-asetukset (kutsutaan joskus MYÖS -määritykseksi), **valitse Vianmääritys > UEFI-laiteohjelmistoasetusten > lisäasetukset.**</span><span class="sxs-lookup"><span data-stu-id="02bac-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="02bac-121">Jos haluat käyttää vikasietotilaa tai muuttaa käynnistyksen lisäasetuksia, **valitse > Käynnistysasetukset >** vianmääritys ja valitse sitten Käynnistä **uudelleen**.</span><span class="sxs-lookup"><span data-stu-id="02bac-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="02bac-122">Sinua saatetaan pyytää antamaan [BitLocker-palautusavain.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)</span><span class="sxs-lookup"><span data-stu-id="02bac-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="02bac-123">Kun tietokone käynnistyy uudelleen, valitse käynnistysasetus, jota haluat käyttää.</span><span class="sxs-lookup"><span data-stu-id="02bac-123">After your PC restarts again, click the startup setting you want to use.</span></span>