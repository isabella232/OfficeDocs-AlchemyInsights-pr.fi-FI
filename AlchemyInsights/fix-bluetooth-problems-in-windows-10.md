---
title: 'Bluetooth-ongelmien korjaaminen Windows 10: ssä'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730156"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="5ff5d-102">Bluetooth-ongelmien korjaaminen Windows 10: ssä</span><span class="sxs-lookup"><span data-stu-id="5ff5d-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="5ff5d-103">Jos Bluetooth-kuvake puuttuu tai Bluetooth-toiminto ei ole käytössä tai sitä ei voi poistaa käytöstä, kannattaa ehkä suorittaa Bluetoothin vian määritys.</span><span class="sxs-lookup"><span data-stu-id="5ff5d-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="5ff5d-104">[Avaa vian määritys-asetukset](ms-settings:troubleshoot), valitse **Bluetooth** **Etsi ja korjaa muut ongelmat**-kohdassa, valitse **Suorita vian määritys**.</span><span class="sxs-lookup"><span data-stu-id="5ff5d-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="5ff5d-105">Jos et näe Bluetooth-kuvaketta, mutta Bluetooth-kuvake tulee näkyviin laite hallintaan:</span><span class="sxs-lookup"><span data-stu-id="5ff5d-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="5ff5d-106">Valitse laite hallinnasta **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="5ff5d-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="5ff5d-107">Paina pitkään (tai napsauta hiiren kakkos painikkeella) Bluetooth-sovittimen nimeä ja valitse **Poista laite**.</span><span class="sxs-lookup"><span data-stu-id="5ff5d-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="5ff5d-108">Sammuta Windows-laite, odota muutama sekunti ja käynnistä se sitten uudelleen.</span><span class="sxs-lookup"><span data-stu-id="5ff5d-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="5ff5d-109">Windows yrittää asentaa ohjaimen uudelleen.</span><span class="sxs-lookup"><span data-stu-id="5ff5d-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="5ff5d-110">Jos olet äskettäin asentanut Windows 10-päivitykset tai päivittänyt Windows 10: een, haluat ehkä tarkistaa ohjainten päivitykset</span><span class="sxs-lookup"><span data-stu-id="5ff5d-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="5ff5d-111">Valitse laite hallinnasta **Bluetooth**ja napsauta sitten Bluetooth-sovittimen nimeä (joka voi sisältää sanan "Radio").</span><span class="sxs-lookup"><span data-stu-id="5ff5d-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="5ff5d-112">Paina Bluetooth-sovitinta pitkään (tai napsauta sitä hiiren kakkos painikkeella) ja valitse sitten **Päivitä**ohjain  >  **haku automaattisesti, jos haluat**päivittää ohjain ohjelmiston.</span><span class="sxs-lookup"><span data-stu-id="5ff5d-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="5ff5d-113">Noudata ohjeita ja valitse sitten **Sulje**.</span><span class="sxs-lookup"><span data-stu-id="5ff5d-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="5ff5d-114">Jos Windows ei löydä uutta Bluetooth-ohjainta, käy tieto koneen valmistajan sivustossa ja lataa uusin Bluetooth-ohjain sieltä.</span><span class="sxs-lookup"><span data-stu-id="5ff5d-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="5ff5d-115">Kun olet ladannut sen, valitse **Päivitä ohjain**  >  **Selaa omaa tieto koneeseeni ohjain ohjelmistoa**  >  **Selaa** sijaintiin, johon ohjain tiedostot on tallennettu > **OK**  >  **Next**ja noudata asennus ohjeita.</span><span class="sxs-lookup"><span data-stu-id="5ff5d-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="5ff5d-116">Kun olet asentanut päivitetyn ohjaimen, Käynnistä tieto kone uudelleen ja tarkista, korjaako se yhteys ongelman.</span><span class="sxs-lookup"><span data-stu-id="5ff5d-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="5ff5d-117">Lisä tietoja Bluetooth-ongelmien vian määrityksestä on artikkelissa koko artikkeli, [Bluetooth-ongelmien korjaaminen Windows 10: ssä](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="5ff5d-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
