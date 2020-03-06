---
title: Käynnistysasetukset Windows 10:ssä
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2020
ms.locfileid: "42409066"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="4151f-102">Käynnistysasetukset Windows 10:ssä</span><span class="sxs-lookup"><span data-stu-id="4151f-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="4151f-103">**Automaattisesti käynnistyksen yhteydessä suoritettavan sovelluksen muuttaminen**</span><span class="sxs-lookup"><span data-stu-id="4151f-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="4151f-104">Siirry [asetukset > Sovellukset > Käynnistys](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="4151f-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="4151f-105">Varmista, että kaikki sovellukset, jotka haluat suorittaa käynnistyksen yhteydessä, ovat **käytössä**.</span><span class="sxs-lookup"><span data-stu-id="4151f-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="4151f-106">**Sovelluksen lisääminen suoritettavaksi automaattisesti käynnistyksen yhteydessä**</span><span class="sxs-lookup"><span data-stu-id="4151f-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="4151f-107">Napsauta tai napauta **Käynnistä** ja etsi sovellus, jonka haluat suorittaa käynnistettäessä.</span><span class="sxs-lookup"><span data-stu-id="4151f-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="4151f-108">Napsauta sovellusta hiiren kakkospainikkeella, valitse **Lisää**ja valitse sitten **Avaa tiedoston sijainti**.</span><span class="sxs-lookup"><span data-stu-id="4151f-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="4151f-109">Tämä avaa sijainnin, johon sovelluksen pikakuvake tallennetaan.</span><span class="sxs-lookup"><span data-stu-id="4151f-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="4151f-110">Jos Avaa tiedostosijainti -asetukselle ei ole vaihtoehtoa, sovellusta ei voi suorittaa käynnistyksen yhteydessä.</span><span class="sxs-lookup"><span data-stu-id="4151f-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="4151f-111">Kun tiedoston sijainti on avoinna, paina **Windows-näppäintä + R**, kirjoita **shell:startup**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="4151f-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="4151f-112">Tämä avaa Käynnistys-kansion.</span><span class="sxs-lookup"><span data-stu-id="4151f-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="4151f-113">Kopioi ja liitä sovelluksen pikakuvake tiedoston sijainnista Käynnistys-kansioon.</span><span class="sxs-lookup"><span data-stu-id="4151f-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="4151f-114">**Käynnistyksen lisäasetukset (mukaan lukien vikasietotila, UEFI-asetukset ja käynnistys toisesta laitteesta)**</span><span class="sxs-lookup"><span data-stu-id="4151f-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="4151f-115">Tallenna työsi ja sulje avoimet asiakirjat, koska nämä vaiheet käynnistävät tietokoneen uudelleen.</span><span class="sxs-lookup"><span data-stu-id="4151f-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="4151f-116">Siirry [kohtaan Asetukset > Päivitys & Suojaus > Recovery](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="4151f-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="4151f-117">Valitse **Käynnistyksen lisäasetukset**-kohdassa **Käynnistä uudelleen nyt**.</span><span class="sxs-lookup"><span data-stu-id="4151f-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="4151f-118">Kun tietokone on käynnistynyt uudelleen Valitse vaihtoehto -näyttöön:</span><span class="sxs-lookup"><span data-stu-id="4151f-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="4151f-119">Jos haluat käynnistää laitteen USB-aseman kaltaiseksi, valitse **Käytä laitetta**.</span><span class="sxs-lookup"><span data-stu-id="4151f-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="4151f-120">Jos haluat syöttää UEFI-asetukset (joita kutsutaan joskus BIOS-asetuksiksi), valitse **> UEFI-laiteohjelmiston asetukset > Lisäasetukset .**</span><span class="sxs-lookup"><span data-stu-id="4151f-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="4151f-121">Jos haluat siirtyä vikasietotilaan tai muuttaa käynnistyksen lisäasetuksia, valitse **Vianmääritys > Lisäasetukset > Käynnistysasetukset**ja valitse sitten **Käynnistä uudelleen**.</span><span class="sxs-lookup"><span data-stu-id="4151f-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="4151f-122">Sinua saatetaan pyytää antamaan [BitLocker-palautusavain](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="4151f-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="4151f-123">Kun tietokone käynnistyy uudelleen, napsauta käynnistysasetusta, jota haluat käyttää.</span><span class="sxs-lookup"><span data-stu-id="4151f-123">After your PC restarts again, click the startup setting you want to use.</span></span>