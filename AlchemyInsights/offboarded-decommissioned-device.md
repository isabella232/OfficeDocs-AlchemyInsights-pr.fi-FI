---
title: Ongelmia käytöstä poistetun tai käytöstä poistetun laitteen poistamisessa Laitevarastosta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564171"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="73332-102">Ongelmia käytöstä poistetun tai käytöstä poistetun laitteen poistamisessa Laitevarastosta</span><span class="sxs-lookup"><span data-stu-id="73332-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="73332-103">Microsoft Defender for Endpoint ei tällä hetkellä salli käytöstä poistetun tai käytöstä poistetun laitteen laitetietueen poistamista laiteluettelosta manuaalisesti.</span><span class="sxs-lookup"><span data-stu-id="73332-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="73332-104">Tietoturvasyistä laite säilyy portaalissa historiatietueena jopa 180 päivän ajan.</span><span class="sxs-lookup"><span data-stu-id="73332-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="73332-105">Laitteen tiedot tyhjenee kuitenkin määritetyn säilytysajan mukaan.</span><span class="sxs-lookup"><span data-stu-id="73332-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="73332-106">**Huomautus:** Käytöstä poistettu tai käytöstä poistettu laite vaihtuu automaattisesti Passiivinen-tilaan **seitsemän** päivän kuluttua.</span><span class="sxs-lookup"><span data-stu-id="73332-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="73332-107">Lisäksi laitteita, jotka eivät ole aktiivisia viimeisten 30 päivän aikana, ei sisällytetä tietoihin, jotka vastaavat organisaatiosi uhkien ja haavoittuvuuksien hallinta tai Microsoft Secure Score for Devices.</span><span class="sxs-lookup"><span data-stu-id="73332-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="73332-108">Jos et edelleenkään halua nähdä tiettyjä laitteita Laitevarasto-näkymässä, kokeile sijoittaa laitetunniste ja suodattaa pois käytöstä poistettu laite Laitevarasto-näkymässä.</span><span class="sxs-lookup"><span data-stu-id="73332-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="73332-109">Lisätietoja on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="73332-109">For more information, see:</span></span>

[<span data-ttu-id="73332-110">Offboard-laitteet Microsoft Defender for Endpoint -palvelusta</span><span class="sxs-lookup"><span data-stu-id="73332-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="73332-111">Valotuspisteet uhkien ja haavoittuvuuksien hallinta</span><span class="sxs-lookup"><span data-stu-id="73332-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="73332-112">Korjaa huonot tunnistimet Microsoft Defender for Endpointissa</span><span class="sxs-lookup"><span data-stu-id="73332-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="73332-113">Tunnisteiden tehokas käyttö (osa 1)</span><span class="sxs-lookup"><span data-stu-id="73332-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="73332-114">Tunnisteiden tehokas käyttö (osa 2)</span><span class="sxs-lookup"><span data-stu-id="73332-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="73332-115">Tunnisteiden tehokas käyttö (osa 3)</span><span class="sxs-lookup"><span data-stu-id="73332-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




