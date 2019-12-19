---
title: Aiemman näytön vian määritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738566"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="3eed7-102">Aiemmin luodun näytön vian määritys</span><span class="sxs-lookup"><span data-stu-id="3eed7-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="3eed7-103">Kokeile näitä ratkaisuja monitorin vian määritykseen.</span><span class="sxs-lookup"><span data-stu-id="3eed7-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="3eed7-104">**Päivitä näytön näyttö:**</span><span class="sxs-lookup"><span data-stu-id="3eed7-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="3eed7-105">Paina seuraavia näppäimiä samanaikaisesti: Windows-näppäin + Ctrl + Shift + B. Tämä päivittää tieto liikenteen näytön ohjaimen kanssa.</span><span class="sxs-lookup"><span data-stu-id="3eed7-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="3eed7-106">Näytöt vilkkuvat hetkellisesti ja tulevat takaisin muutaman sekunnin kuluttua.</span><span class="sxs-lookup"><span data-stu-id="3eed7-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="3eed7-107">**Valvonta laitteiston vian määritys:**</span><span class="sxs-lookup"><span data-stu-id="3eed7-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="3eed7-108">Irrota kaapeli, joka yhdistää tieto koneen näyttöön, ja kytke se takaisin.</span><span class="sxs-lookup"><span data-stu-id="3eed7-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="3eed7-109">Irrota kaikki muut kuin olennaiset laitteet tieto koneesta (kuten sovittimet tai telakat).</span><span class="sxs-lookup"><span data-stu-id="3eed7-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="3eed7-110">**Jos olet hiljattain asentanut päivityksen tieto koneeseesi, voit palauttaa näytön ohjaimen:**</span><span class="sxs-lookup"><span data-stu-id="3eed7-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="3eed7-111">Valitse **Aloitus**, kirjoita **laite hallinta**ja valitse tuloksista **laite hallinta** .</span><span class="sxs-lookup"><span data-stu-id="3eed7-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="3eed7-112">Laajenna **näyttö sovittimet** -osa, napsauta näyttö sovitinta hiiren kakkos painikkeella ja valitse **Ominaisuudet**.</span><span class="sxs-lookup"><span data-stu-id="3eed7-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="3eed7-113">Siirry **ohjain** -väli lehdelle ja valitse **Aikaisempi ohjain**.</span><span class="sxs-lookup"><span data-stu-id="3eed7-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="3eed7-114">Huomautus: Jos tämä ei ole käytettävissä tai se näkyy harmaana, siirry seuraavaan vaiheeseen valitsemalla alla olevista vaihto ehdoista **ei** .</span><span class="sxs-lookup"><span data-stu-id="3eed7-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="3eed7-115">Sinun on ehkä käynnistettävä tieto kone uudelleen, ennen kuin nämä muutokset tulevat voimaan.</span><span class="sxs-lookup"><span data-stu-id="3eed7-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="3eed7-116">**Poista näytön ohjaimen asennus ja asenna se uudelleen:**</span><span class="sxs-lookup"><span data-stu-id="3eed7-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="3eed7-117">Valitse **Aloitus**, kirjoita **laite hallinta**ja valitse tuloksista **laite hallinta** .</span><span class="sxs-lookup"><span data-stu-id="3eed7-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="3eed7-118">Laajenna **näyttö sovittimet** -osa, napsauta näyttö sovitinta hiiren kakkos painikkeella ja valitse **Poista laitteen asennus**.</span><span class="sxs-lookup"><span data-stu-id="3eed7-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="3eed7-119">Valitse **Poista tämän laitteen ohjain ohjelmisto** -valinta ruutu ja valitse **Poista asennus**.</span><span class="sxs-lookup"><span data-stu-id="3eed7-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="3eed7-120">Huomautus: sinua saatetaan pyytää käynnistämään tieto kone uudelleen tässä vaiheessa.</span><span class="sxs-lookup"><span data-stu-id="3eed7-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="3eed7-121">Muista kirjoittaa loput ohjeet ennen uudelleenkäynnistystä.</span><span class="sxs-lookup"><span data-stu-id="3eed7-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="3eed7-122">Avaa laite hallinta uudelleen.</span><span class="sxs-lookup"><span data-stu-id="3eed7-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="3eed7-123">Laajenna **näyttö sovittimet** -osio, napsauta näyttö sovitinta hiiren kakkos painikkeella ja valitse **Päivitä ohjain**.</span><span class="sxs-lookup"><span data-stu-id="3eed7-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="3eed7-124">Valitse **Hae automaattisesti päivitetäänkö ohjain ohjelmisto** ja noudata asennus ohjeita.</span><span class="sxs-lookup"><span data-stu-id="3eed7-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>