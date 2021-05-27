---
title: Ohjelmistoluettelo puuttuu tai se on virheellinen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676264"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="e5aef-102">Ohjelmistoluettelo puuttuu tai se on virheellinen</span><span class="sxs-lookup"><span data-stu-id="e5aef-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="e5aef-103">Uhkien ja haavoittuvuuksien hallinta (TVM) -ohjelman sovellusluettelo on luettelo organisaatiosi tunnetuista ohjelmistoista, joissa on virallisia Common Platform Enumerations (CPE) -luetteloita.</span><span class="sxs-lookup"><span data-stu-id="e5aef-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="e5aef-104">Ohjelmistotuotteissa, joissa ei ole virallista CPE:tä, ei ole julkaistu tietoturva-aukkoja.</span><span class="sxs-lookup"><span data-stu-id="e5aef-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="e5aef-105">Varasto sisältää myös tietoja, kuten toimittajan nimen, heikkouksien määrän, uhat ja laitteiden määrän.</span><span class="sxs-lookup"><span data-stu-id="e5aef-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="e5aef-106">Laitteiden ohjelmistomuutokset näkyvät yleensä suojausportaaleissa kahden tunnin kuluessa.</span><span class="sxs-lookup"><span data-stu-id="e5aef-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="e5aef-107">Tämä voi kuitenkin joskus kestää kauemmin.</span><span class="sxs-lookup"><span data-stu-id="e5aef-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="e5aef-108">Tällä hetkellä synkronointia ei voi pakottaa. tämä on jatkuva jatkuva arviointi.</span><span class="sxs-lookup"><span data-stu-id="e5aef-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="e5aef-109">Jos olet tehnyt ohjelmistopäivityksen, eikä muutos näy oikein TVM:ssä viiden tunnin kuluttua, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="e5aef-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="e5aef-110">Tarkista ohjelmiston todistusaineisto-osasta, miten ohjelmisto on havaittu.</span><span class="sxs-lookup"><span data-stu-id="e5aef-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="e5aef-111">Varmista, että ohjelmisto on tuettu.</span><span class="sxs-lookup"><span data-stu-id="e5aef-111">Make sure that the software is supported.</span></span> <span data-ttu-id="e5aef-112">Ohjelmisto saattaa olla näkyvissä vain laitetasolla, vaikka ohjelmisto ei tällä hetkellä tue uhkien ja haavoittuvuuksien hallinta.</span><span class="sxs-lookup"><span data-stu-id="e5aef-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="e5aef-113">Saatavilla on kuitenkin vain rajoitettuja tietoja.</span><span class="sxs-lookup"><span data-stu-id="e5aef-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="e5aef-114">Vaiheita, joissa raportoit epätarkkuuksesta portaalissa, on kohdassa [Epätarkkuuksesta ilmoittaminen.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)</span><span class="sxs-lookup"><span data-stu-id="e5aef-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="e5aef-115">**Huomautus:** MDE-portaalin epätarkkuuksia raportoiminen on yksi tapa lisätä suunnittelua.</span><span class="sxs-lookup"><span data-stu-id="e5aef-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="e5aef-116">Jos ongelma on kiireellinen, avaa tukipalvelupyynnön.</span><span class="sxs-lookup"><span data-stu-id="e5aef-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="e5aef-117">Lisätietoja on kohdassa Ohjelmistovarasto [– uhkien ja haavoittuvuuksien hallinta.](/microsoft-365/security/defender-endpoint/tvm-software-inventory)</span><span class="sxs-lookup"><span data-stu-id="e5aef-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>