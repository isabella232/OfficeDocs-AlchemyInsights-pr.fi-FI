---
title: Kalenteritapahtumat puuttuvat tai eivät päivity
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: b114411d6285a68a41bbcbf64151c212ee2cf661
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51837190"
---
# <a name="calendar-events-missing-or-not-updating"></a><span data-ttu-id="9d482-102">Kalenteritapahtumat puuttuvat tai eivät päivity</span><span class="sxs-lookup"><span data-stu-id="9d482-102">Calendar Events missing or not updating</span></span>

<span data-ttu-id="9d482-103">Jos kalenterikohteita puuttuu tai ne eivät päivity, aloita tarkastelemalla kalenterikansion ominaisuuksien kohteiden lukumäärää Outlookissa:</span><span class="sxs-lookup"><span data-stu-id="9d482-103">If calendar items are missing or not updating, start by looking at the item count in your Calendar folder properties in Outlook:</span></span> 

1. <span data-ttu-id="9d482-104">Napsauta käyttäjän Kalenteri-kansiota **hiiren kakkospainikkeella** ja valitse **ominaisuudet**.</span><span class="sxs-lookup"><span data-stu-id="9d482-104">Right-click on the affected user **Calendar** folder, and then select **Properties**.</span></span>

1. <span data-ttu-id="9d482-105">Valitse **Synkronointi-välilehti.**</span><span class="sxs-lookup"><span data-stu-id="9d482-105">Select the **Synchronization** tab.</span></span>

<span data-ttu-id="9d482-106">Jos kohteiden määrä ei ole sama palvelinkansion ja offline-kansion välillä:</span><span class="sxs-lookup"><span data-stu-id="9d482-106">If the item count is not the same between the Server folder and the Offline Folder:</span></span>

1.  <span data-ttu-id="9d482-107">Korosta **Kalenteri-kansio.**</span><span class="sxs-lookup"><span data-stu-id="9d482-107">Highlight the **Calendar** folder.</span></span>

1.  <span data-ttu-id="9d482-108">Siirry Lähetä **vastaanotto** / **-välilehteen** ja valitse Päivitä **kansio**.</span><span class="sxs-lookup"><span data-stu-id="9d482-108">Go to the **Send**/**Receive** tab, and then select **Update Folder**.</span></span>

<span data-ttu-id="9d482-109">Jos kalenterisi ei edelleenkään päivity tai tapahtumat puuttuvat, lataa Outlookin kalenterin tarkistustyökalu [Microsoft download centeristä](https://www.microsoft.com/download/details.aspx?id=28786).</span><span class="sxs-lookup"><span data-stu-id="9d482-109">If your calendar is still not updating or events are missing, download the Calendar Checking Tool for Outlook from the [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=28786).</span></span> <span data-ttu-id="9d482-110">Selvitä, onko kalenterikansiossa yli 5 000 kohdetta, sillä tämä voi aiheuttaa ongelmia, kuten kalenterikokouksia ei päivitetä tai kokousvirheitä.</span><span class="sxs-lookup"><span data-stu-id="9d482-110">Determine if there are more than 5000 items in the calendar folder as this can cause symptoms such as calendar meetings not updated or meeting errors.</span></span> 

<span data-ttu-id="9d482-111">Lisätietoja on kohdassa [Outlookin suorituskykyongelmat, kun](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders)välimuistitilassa .ost- tai .pst-tiedostossa on liikaa kohteita tai kansioita.</span><span class="sxs-lookup"><span data-stu-id="9d482-111">For more information, see [Outlook performance issues when there are too many items or folders in a cached mode .ost or .pst file](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span></span>