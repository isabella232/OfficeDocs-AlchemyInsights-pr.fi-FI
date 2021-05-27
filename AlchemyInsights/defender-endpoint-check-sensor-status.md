---
title: Defender endpointin tarkistustunnistimen tila
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676181"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="dd604-102">Defender endpointin tarkistustunnistimen tila</span><span class="sxs-lookup"><span data-stu-id="dd604-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="dd604-103">Laitteet, **joissa on tunnistimen ongelmat** -ruutu, on Security Operations -koontinäytössä.</span><span class="sxs-lookup"><span data-stu-id="dd604-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="dd604-104">Tässä ruudussa on tietoja siitä, miten yksittäinen laite voi tarjota tunnistimen tietoja ja viestiä Defender for Endpoint -palvelun kanssa.</span><span class="sxs-lookup"><span data-stu-id="dd604-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="dd604-105">Se ilmoittaa, kuinka moneen laitteeseen on kiinnitettävä huomiota, auttaa tunnistamaan ongelmalaitteet ja korjaamaan tunnetut ongelmat.</span><span class="sxs-lookup"><span data-stu-id="dd604-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="dd604-106">Ruudussa on kaksi tilailmaisinta, jotka ilmoittavat siitä, kuinka monta laitetta ei ole ilmoittanut asianmukaisesti palvelulle:</span><span class="sxs-lookup"><span data-stu-id="dd604-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="dd604-107">**Määritetty väärin** Laitteet, jotka saattavat raportoida tunnistimen tiedoista osittain Defender for Endpoint -palveluun ja joissa voi olla kokoonpanovirheitä, jotka on korjattava.</span><span class="sxs-lookup"><span data-stu-id="dd604-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="dd604-108">**Passiivinen** Laitteet, jotka ovat lopenneet raportoinnin Defender for Endpoint -palveluun yli seitsemän päivän ajan viimeisen kuukauden aikana.</span><span class="sxs-lookup"><span data-stu-id="dd604-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="dd604-109">Kun napsautat mitä tahansa ryhmää, sinut ohjataan Laitteet-luetteloon valintojen mukaan suodatettuna.</span><span class="sxs-lookup"><span data-stu-id="dd604-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="dd604-110">Laitteet-luettelossa voit suodattaa kuntotilaluettelon seuraavan tilan mukaan:</span><span class="sxs-lookup"><span data-stu-id="dd604-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="dd604-111">**Aktiivinen** Laitteet, jotka raportoivat aktiivisesti Defender for Endpoint -palveluun.</span><span class="sxs-lookup"><span data-stu-id="dd604-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="dd604-112">**Määritetty väärin** Laitteet, jotka saattavat raportoida tunnistimen tiedoista osittain Defender for Endpoint -palveluun, mutta joissa on kokoonpanovirheitä, jotka on korjattava.</span><span class="sxs-lookup"><span data-stu-id="dd604-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="dd604-113">Virheellisesti määritetyt laitteet voivat sisältää joko yhden seuraavista ongelmista tai niiden yhdistelmän:</span><span class="sxs-lookup"><span data-stu-id="dd604-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="dd604-114">Ei tunnistintietoja – Laitteet ovat lopetta tunnistimen tietojen lähettämisen.</span><span class="sxs-lookup"><span data-stu-id="dd604-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="dd604-115">Laitteesta voidaan käynnistää rajoitettuja ilmoituksia.</span><span class="sxs-lookup"><span data-stu-id="dd604-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="dd604-116">Heikentynyt viestintä – Viestintä laitteen kanssa on heikentynyt.</span><span class="sxs-lookup"><span data-stu-id="dd604-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="dd604-117">Tiedostojen lähettäminen syvällistä analyysia varten, tiedostojen estäminen, laitteen eristäminen verkosta ja muut toiminnot, jotka edellyttävät viestintää laitteen kanssa, eivät ehkä toimi.</span><span class="sxs-lookup"><span data-stu-id="dd604-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="dd604-118">**Passiivinen** Laitteet, jotka ovat lopetta raportoinnin Defender for Endpoint -palveluun.</span><span class="sxs-lookup"><span data-stu-id="dd604-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="dd604-119">Voit ladata koko luettelon CSV-muodossa Vie-toiminnolla.</span><span class="sxs-lookup"><span data-stu-id="dd604-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="dd604-120">Lisätietoja on kohdassa [Sensorin tilan tarkastaminen Microsoft Defender for Endpointissa.](/microsoft-365/security/defender-endpoint/check-sensor-status)</span><span class="sxs-lookup"><span data-stu-id="dd604-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="dd604-121">Lisätietoja siitä, mikä aiheutti laitteen passiivisen tai virheellisen määrityksen, on kohdassa Korjaa huonosti toimivat tunnistimet [Microsoft Defender for Endpointissa.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)</span><span class="sxs-lookup"><span data-stu-id="dd604-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
