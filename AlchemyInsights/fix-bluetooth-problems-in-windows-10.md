---
title: Bluetooth-ongelmien ratkaiseminen Windows 10:ssä
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
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812929"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="ac8ef-102">Bluetooth-ongelmien ratkaiseminen Windows 10:ssä</span><span class="sxs-lookup"><span data-stu-id="ac8ef-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="ac8ef-103">Jos Bluetooth-kuvake puuttuu tai Bluetoothia ei voi ottaa käyttöön tai poistaa käytöstä, voit suorittaa Bluetooth-vianmäärityksen.</span><span class="sxs-lookup"><span data-stu-id="ac8ef-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="ac8ef-104">[Avaa Vianmääritysasetukset ,](ms-settings:troubleshoot)valitse Etsi ja korjaa muita ongelmia **-kohdassa** **Bluetooth** ja valitse **Suorita vianmääritys**.</span><span class="sxs-lookup"><span data-stu-id="ac8ef-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="ac8ef-105">Jos et näe Bluetooth-kuvaketta, mutta Bluetooth näkyy Laitehallinnassa:</span><span class="sxs-lookup"><span data-stu-id="ac8ef-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="ac8ef-106">Valitse Laitehallinnassa **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="ac8ef-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="ac8ef-107">Paina pitkään (tai napsauta hiiren kakkospainikkeella) Bluetooth-sovittimen nimeä ja valitse **Poista laitteen asennus**.</span><span class="sxs-lookup"><span data-stu-id="ac8ef-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="ac8ef-108">Sammuta Windows-laite, odota muutama sekunti ja käynnistä se sitten uudelleen.</span><span class="sxs-lookup"><span data-stu-id="ac8ef-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="ac8ef-109">Windows yrittää asentaa ohjaimen uudelleen.</span><span class="sxs-lookup"><span data-stu-id="ac8ef-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="ac8ef-110">Jos olet hiljattain asentanut Windows 10:n päivitykset tai päivittänyt Windows 10:ksi, voit tarkistaa ohjainpäivitykset:</span><span class="sxs-lookup"><span data-stu-id="ac8ef-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="ac8ef-111">Valitse Laitehallinnassa **Bluetooth** ja napsauta sitten Bluetooth-sovittimen nimeä (joka voi sisältää sanan "radio").</span><span class="sxs-lookup"><span data-stu-id="ac8ef-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="ac8ef-112">Paina pitkään (tai napsauta hiiren kakkospainikkeella) Bluetooth-sovitinta ja valitse sitten **Päivitä** ohjainhaku automaattisesti  >  **päivitetyn ohjainohjelmiston varalta.**</span><span class="sxs-lookup"><span data-stu-id="ac8ef-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="ac8ef-113">Noudata ohjeita ja valitse **sitten Sulje**.</span><span class="sxs-lookup"><span data-stu-id="ac8ef-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="ac8ef-114">Jos Windows ei löydä uutta Bluetooth-ohjainta, siirry tietokoneen valmistajan sivustoon ja lataa uusin Bluetooth-ohjain sieltä.</span><span class="sxs-lookup"><span data-stu-id="ac8ef-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="ac8ef-115">Kun olet ladanut ohjaimen, valitse Päivitä ohjain Selaa tietokoneeni ohjainohjelmistoa Etsi sijainti, johon ohjaintiedostot   >    >   on tallennettu, > **OK**  >  **Seuraava**, ja asenna se noudattamalla ohjeita.</span><span class="sxs-lookup"><span data-stu-id="ac8ef-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="ac8ef-116">Kun olet asentanut päivitetyn ohjaimen, käynnistä tietokone uudelleen ja tarkista, korjaako se yhteysongelman.</span><span class="sxs-lookup"><span data-stu-id="ac8ef-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="ac8ef-117">Lisätietoja Bluetooth-ongelmien vianmäärityksestä on koko artikkelissa [Bluetooth-ongelmien ratkaiseminen Windows 10:ssä.](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)</span><span class="sxs-lookup"><span data-stu-id="ac8ef-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
