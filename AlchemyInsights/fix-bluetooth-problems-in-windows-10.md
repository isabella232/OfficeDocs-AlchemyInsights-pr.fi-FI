---
title: Bluetooth-ongelmien korjaaminen Windows 10:ssä
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 94dda7a42632f57ce3aef5f467b87df1033b8d49
ms.sourcegitcommit: 9a35768444824cde9e192f1d9daafc9157437244
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268631"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="90bd0-102">Bluetooth-ongelmien korjaaminen Windows 10:ssä</span><span class="sxs-lookup"><span data-stu-id="90bd0-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="90bd0-103">Jos Bluetooth-kuvake puuttuu tai Bluetooth ei voi ottaa käyttöön tai poistaa sitä käytöstä, voit suorittaa Bluetooth-vianmäärityksen.</span><span class="sxs-lookup"><span data-stu-id="90bd0-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="90bd0-104">[Avaa Vianmääritysasetukset](ms-settings:troubleshoot), valitse **Etsi ja korjaa muita ongelmia**-kohdasta **Bluetooth** ja valitse Suorita **vianmääritys**.</span><span class="sxs-lookup"><span data-stu-id="90bd0-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="90bd0-105">Jos Bluetooth-kuvaketta ei näy, mutta Bluetooth näkyy Laitehallinnassa:</span><span class="sxs-lookup"><span data-stu-id="90bd0-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="90bd0-106">Valitse Laitehallinnassa **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="90bd0-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="90bd0-107">Paina Bluetooth-sovittimen nimeä pitkään (tai napsauta sitä hiiren kakkospainikkeella) ja valitse **Poista laitteen asennus**.</span><span class="sxs-lookup"><span data-stu-id="90bd0-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="90bd0-108">Sammuta Windows-laite, odota muutama sekunti ja käynnistä se sitten uudelleen.</span><span class="sxs-lookup"><span data-stu-id="90bd0-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="90bd0-109">Windows yrittää asentaa ohjaimen uudelleen.</span><span class="sxs-lookup"><span data-stu-id="90bd0-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="90bd0-110">Jos olet äskettäin asentanut Windows 10 -päivitykset tai päivittänyt Windows 10:een, voit tarkistaa ohjainpäivitykset:</span><span class="sxs-lookup"><span data-stu-id="90bd0-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="90bd0-111">Valitse Laitehallinnassa **Bluetooth**ja napsauta sitten Bluetooth-sovittimen nimeä (joka voi sisältää sanan "radio").</span><span class="sxs-lookup"><span data-stu-id="90bd0-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="90bd0-112">Paina Bluetooth-sovitinta pitkään (tai napsauta sitä hiiren kakkospainikkeella) ja valitse sitten **Päivitä ohjainhaku** > **automaattisesti päivitetylle ohjainohjelmistolle**.</span><span class="sxs-lookup"><span data-stu-id="90bd0-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="90bd0-113">Noudata ohjeita ja valitse sitten **Sulje**.</span><span class="sxs-lookup"><span data-stu-id="90bd0-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="90bd0-114">Jos Windows ei löydä uutta Bluetooth-ohjainta, käy tietokoneen valmistajan sivustossa ja lataa sieltä uusin Bluetooth-ohjain.</span><span class="sxs-lookup"><span data-stu-id="90bd0-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="90bd0-115">Kun olet ladannut sen, valitse **Päivitä ohjain** > **Selaa tietokoneen ohjainohjelmistoa** > **Etsi sijainti,** johon ohjaintiedostot on tallennettu > **OK** > **Seuraava**, ja noudata asennusohjeita.</span><span class="sxs-lookup"><span data-stu-id="90bd0-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="90bd0-116">Kun olet asentanut päivitetyn ohjaimen, käynnistä laite uudelleen ja tarkista, korjaako se yhteysongelman.</span><span class="sxs-lookup"><span data-stu-id="90bd0-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="90bd0-117">Lisätietoja Bluetooth-ongelmien vianmäärityksestä on windows 10:n koko artikkelissa [Bluetooth-ongelmien korjaaminen](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="90bd0-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
