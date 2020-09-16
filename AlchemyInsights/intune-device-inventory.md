---
title: Intune-laitteen luettelointi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667875"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="1442f-102">Intune-laitteen luettelointi</span><span class="sxs-lookup"><span data-stu-id="1442f-102">Intune Device Inventory</span></span>

<span data-ttu-id="1442f-103">Laitteet-Blade tarjoaa hallinnoijan käsityksen laitteista, jotka ovat hallinta-kohdassa Intunella laitekohtaisesti.</span><span class="sxs-lookup"><span data-stu-id="1442f-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="1442f-104">Näytetyt tiedot sisältävät: laitteisto, löydetyt sovellukset, laitteen yhteensopivuus tila ja laitteen määritys tila.</span><span class="sxs-lookup"><span data-stu-id="1442f-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="1442f-105">Laitteiston ja löydettyjen sovellusten varasto tiedot kerätään seitsemän päivän jaksolle.</span><span class="sxs-lookup"><span data-stu-id="1442f-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="1442f-106">Sovellusten ja laitteiden tietyt ominaisuudet on ilmoitettu eri tavalla laitteen käyttö järjestelmän mukaan ja sen mukaan, onko laite henkilökohtaisesti vai yrityksen omistama.</span><span class="sxs-lookup"><span data-stu-id="1442f-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="1442f-107">Lisä tietoja on kohdassa [laitteen tietojen tarkasteleminen Intunella](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="1442f-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="1442f-108">**Usein kysytyt kysymykset**</span><span class="sxs-lookup"><span data-stu-id="1442f-108">**FAQ**</span></span>

<span data-ttu-id="1442f-109">K: en saa täyttä luetteloa sovelluksista, jotka esiintyvät Intune-kirjoilla Windows-laitteissa.</span><span class="sxs-lookup"><span data-stu-id="1442f-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="1442f-110">Miksi ei?</span><span class="sxs-lookup"><span data-stu-id="1442f-110">Why not?</span></span>

<span data-ttu-id="1442f-111">A: tällä hetkellä vain nykyaikaisia sovelluksia on lueteltu Windows 10-tieto koneissa, jotka tunnistetaan yritys laitteiksi.</span><span class="sxs-lookup"><span data-stu-id="1442f-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="1442f-112">Intune ei kerää tietoja näihin laitteisiin asenne tuista Win32-sovelluksista.</span><span class="sxs-lookup"><span data-stu-id="1442f-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="1442f-113">K: Miksi Puhelin numeroita ei ole kerätty kaikista laitteista?</span><span class="sxs-lookup"><span data-stu-id="1442f-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="1442f-114">A: Intunen yritys käyttöön luokiteltuja puhelimia ei ole tunnistettu koko Puhelin numeroksi, kun suoritat esimerkiksi mobiililaitteiden inventaario raportin.</span><span class="sxs-lookup"><span data-stu-id="1442f-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="1442f-115">Tuo sinulle-laitteen Puhelin numerot on aina osittain peitetty tähdellä (\* \* \* \*) ja näyttää vain viimeiset neljä numeroa.</span><span class="sxs-lookup"><span data-stu-id="1442f-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>