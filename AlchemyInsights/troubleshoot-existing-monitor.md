---
title: Olemassa olevan näytön vian määritys
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
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690708"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="f3290-102">Aiemmin luodun näytön vian määritys</span><span class="sxs-lookup"><span data-stu-id="f3290-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="f3290-103">Kokeile näitä ratkaisuja näytön vian määritykseen.</span><span class="sxs-lookup"><span data-stu-id="f3290-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="f3290-104">**Näytön näytön päivittäminen:**</span><span class="sxs-lookup"><span data-stu-id="f3290-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="f3290-105">Paina yhtä aikaa seuraavia näppäimiä: Windows-näppäin + Ctrl + vaihto + B. Tämä päivittää tieto liikenteen näytön ohjaimen kanssa.</span><span class="sxs-lookup"><span data-stu-id="f3290-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="f3290-106">Näytöt vilkkuvat hetkellisesti ja palaavat muutaman sekunnin kuluttua.</span><span class="sxs-lookup"><span data-stu-id="f3290-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="f3290-107">**Valvonta laitteiden vian määritys:**</span><span class="sxs-lookup"><span data-stu-id="f3290-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="f3290-108">Irrota kaapeli, joka yhdistää tieto koneen monitorien ja kytke se takaisin.</span><span class="sxs-lookup"><span data-stu-id="f3290-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="f3290-109">Irrota tieto koneesta kaikki muut kuin tärkeät laitteet (kuten sovittimet tai telakat).</span><span class="sxs-lookup"><span data-stu-id="f3290-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="f3290-110">**Jos olet äskettäin asentanut päivityksen tieto KONEESEESI, voit palauttaa näyttö ohjaimen seuraavasti:**</span><span class="sxs-lookup"><span data-stu-id="f3290-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="f3290-111">Valitse **Käynnistä**, kirjoita **laite hallintaan**ja valitse tuloksista **laite hallintaa** .</span><span class="sxs-lookup"><span data-stu-id="f3290-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="f3290-112">Laajenna **näyttö sovittimet** -kohta, napsauta näyttösovittimesi hiiren kakkos painikkeella ja valitse **Ominaisuudet**.</span><span class="sxs-lookup"><span data-stu-id="f3290-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="f3290-113">Siirry **ohjain** -väli lehteen ja valitse **Edellinen ohjain**.</span><span class="sxs-lookup"><span data-stu-id="f3290-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="f3290-114">Huomautus: Jos tämä ei ole käytettävissä tai se näkyy harmaana, siirry seuraavaan vaiheeseen valitsemalla **ei** alla olevista vaihto ehdoista.</span><span class="sxs-lookup"><span data-stu-id="f3290-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="f3290-115">Sinun on ehkä käynnistettävä tieto kone uudelleen, ennen kuin muutokset tulevat voimaan.</span><span class="sxs-lookup"><span data-stu-id="f3290-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="f3290-116">**Poista näyttö ohjaimen asennus ja asenna se uudelleen:**</span><span class="sxs-lookup"><span data-stu-id="f3290-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="f3290-117">Valitse **Käynnistä**, kirjoita **laite hallintaan**ja valitse tuloksista **laite hallintaa** .</span><span class="sxs-lookup"><span data-stu-id="f3290-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="f3290-118">Laajenna **näyttö sovittimet** -kohta, napsauta näyttösovittimesi hiiren kakkos painikkeella, valitse **Poista laite**.</span><span class="sxs-lookup"><span data-stu-id="f3290-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="f3290-119">Valitse **Poista tämän laitteen ohjain ohjelmisto** -kohdan vieressä oleva valinta ruutu ja valitse **Poista asennus**.</span><span class="sxs-lookup"><span data-stu-id="f3290-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="f3290-120">Huomautus: sinua saatetaan pyytää käynnistämään tieto kone uudelleen tässä vaiheessa.</span><span class="sxs-lookup"><span data-stu-id="f3290-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="f3290-121">Muista kirjoittaa jäljellä olevat ohjeet muistiin ennen uudelleenkäynnistystä.</span><span class="sxs-lookup"><span data-stu-id="f3290-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="f3290-122">Avaa laite hallintaa uudelleen.</span><span class="sxs-lookup"><span data-stu-id="f3290-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="f3290-123">Laajenna **näyttö sovittimet** -kohta, napsauta näyttösovittimesi hiiren kakkos painikkeella ja valitse **Päivitä ohjain**.</span><span class="sxs-lookup"><span data-stu-id="f3290-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="f3290-124">Valitse **Päivitä ohjain ohjelmisto automaattisesti** -kohdassa haku ja noudata asennus ohjeita.</span><span class="sxs-lookup"><span data-stu-id="f3290-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>