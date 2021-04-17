---
title: Olemassa olevan näytön vianmääritys
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824576"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="74e62-102">Olemassa olevan näytön vianmääritys</span><span class="sxs-lookup"><span data-stu-id="74e62-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="74e62-103">Kokeile näitä ratkaisuja näytön vianmääritykseen.</span><span class="sxs-lookup"><span data-stu-id="74e62-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="74e62-104">**Päivitä näyttösi näyttö:**</span><span class="sxs-lookup"><span data-stu-id="74e62-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="74e62-105">Paina samanaikaisesti seuraavia näppäimiä: Windows-näppäin + Ctrl + Vaihto + B. Tämä päivittää tietoliikenteen grafiikkaohjaimen kanssa.</span><span class="sxs-lookup"><span data-stu-id="74e62-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="74e62-106">Näytöt vilkkuvat hetkellisesti ja palaavat muutaman sekunnin kuluttua.</span><span class="sxs-lookup"><span data-stu-id="74e62-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="74e62-107">**Monitorin laitteiston vianmääritys:**</span><span class="sxs-lookup"><span data-stu-id="74e62-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="74e62-108">Irrota kaapeli, joka yhdistää tietokoneen näyttöön, ja kytke se takaisin sisään.</span><span class="sxs-lookup"><span data-stu-id="74e62-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="74e62-109">Irrota kaikki muut kuin tärkeät laitteet tietokoneesta (kuten sovittimet tai telakalla).</span><span class="sxs-lookup"><span data-stu-id="74e62-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="74e62-110">**Jos olet hiljattain asentanut tietokoneeseen päivityksen, voit ottaa näyttöohjaimen takaisin näkyviin:**</span><span class="sxs-lookup"><span data-stu-id="74e62-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="74e62-111">Valitse **Käynnistä**, kirjoita **laitehallinta** ja **valitse tuloksista** Laitehallinta.</span><span class="sxs-lookup"><span data-stu-id="74e62-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="74e62-112">Laajenna **Näyttösovittimet-osa,** napsauta näyttösovitinta hiiren kakkospainikkeella ja valitse **Ominaisuudet**.</span><span class="sxs-lookup"><span data-stu-id="74e62-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="74e62-113">Siirry **Ohjain-välilehteen** ja valitse **Roll Back Driver (Takaisinohjain).**</span><span class="sxs-lookup"><span data-stu-id="74e62-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="74e62-114">Huomautus: Jos tämä ei ole käytettävissä tai se  näkyy harmaana, siirry seuraavaan vaiheeseen valitsemalla alla olevista vaihtoehdoista Ei.</span><span class="sxs-lookup"><span data-stu-id="74e62-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="74e62-115">Tietokone on ehkä käynnistettävä uudelleen, ennen kuin muutokset tulevat voimaan.</span><span class="sxs-lookup"><span data-stu-id="74e62-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="74e62-116">**Poista näyttöohjain ja asenna se uudelleen:**</span><span class="sxs-lookup"><span data-stu-id="74e62-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="74e62-117">Valitse **Käynnistä**, kirjoita **laitehallinta** ja **valitse tuloksista** Laitehallinta.</span><span class="sxs-lookup"><span data-stu-id="74e62-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="74e62-118">Laajenna **Näyttösovittimet-osa,** napsauta näyttösovitinta hiiren kakkospainikkeella ja valitse **Poista laitteen asennus**.</span><span class="sxs-lookup"><span data-stu-id="74e62-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="74e62-119">Valitse kohdan Poista **tämän laitteen ohjainohjelmistot vieressä olevaa ruutua** ja valitse **Poista asennus**.</span><span class="sxs-lookup"><span data-stu-id="74e62-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="74e62-120">Huomautus: Sinua saatetaan pyytää käynnistämään tietokone uudelleen tässä vaiheessa.</span><span class="sxs-lookup"><span data-stu-id="74e62-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="74e62-121">Muista kirjoittaa loput ohjeet muistiin ennen uudelleenkäynnistystä.</span><span class="sxs-lookup"><span data-stu-id="74e62-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="74e62-122">Avaa Laitehallinta uudelleen.</span><span class="sxs-lookup"><span data-stu-id="74e62-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="74e62-123">Laajenna **Näyttösovittimet-osa,** napsauta näyttösovitinta hiiren kakkospainikkeella ja valitse **Päivitä ohjain**.</span><span class="sxs-lookup"><span data-stu-id="74e62-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="74e62-124">Valitse **Etsi ohjainohjelmisto automaattisesti ja** noudata asennusohjeita.</span><span class="sxs-lookup"><span data-stu-id="74e62-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>