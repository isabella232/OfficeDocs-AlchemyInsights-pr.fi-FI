---
title: Intune Laitteen varasto
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439653"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="b41b7-102">Intune Laitteen varasto</span><span class="sxs-lookup"><span data-stu-id="b41b7-102">Intune Device Inventory</span></span>

<span data-ttu-id="b41b7-103">Laitteet-terä antaa järjestelmänvalvojan käsityksen Intunen hallinnassa olevista laitteista laitekohtaisesti.</span><span class="sxs-lookup"><span data-stu-id="b41b7-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="b41b7-104">Näytettyjä tietoja ovat: Laitteisto, Löydetyt sovellukset, Laitevaatimustenmukaisuuden tila ja Laiteasetukset-tila.</span><span class="sxs-lookup"><span data-stu-id="b41b7-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="b41b7-105">Laitteiston ja löydettyjen sovellusten varastotiedot kerätään seitsemän päivän jakson aikana.</span><span class="sxs-lookup"><span data-stu-id="b41b7-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="b41b7-106">Raportoidut sovellukset ja laitteiston erityiselementit vaihtelevat laitteen käyttöjärjestelmän ja sen mukaan, onko laite henkilökohtaisesti vai yrityksen omistuksessa.</span><span class="sxs-lookup"><span data-stu-id="b41b7-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="b41b7-107">Lisätietoja on kohdassa [Laitteen tiedot kohdassa Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="b41b7-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="b41b7-108">**Usein kysytyt kysymykset**</span><span class="sxs-lookup"><span data-stu-id="b41b7-108">**FAQ**</span></span>

<span data-ttu-id="b41b7-109">K: En saa täydellistä luetteloa Intune-rekisteröimistä Windows-laitteista olevista sovelluksista.</span><span class="sxs-lookup"><span data-stu-id="b41b7-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="b41b7-110">Miksi ei?</span><span class="sxs-lookup"><span data-stu-id="b41b7-110">Why not?</span></span>

<span data-ttu-id="b41b7-111">: Tällä hetkellä vain nykyaikaiset sovellukset on lueteltu Windows 10 -tietokoneissa, jotka on tunnistettu yrityslaitteisiksi.</span><span class="sxs-lookup"><span data-stu-id="b41b7-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="b41b7-112">Intune ei kerää tietoja näihin laitteisiin asennetuista Win32-sovelluksista.</span><span class="sxs-lookup"><span data-stu-id="b41b7-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="b41b7-113">K: Miksi puhelinnumeroita ei kerätä kaikista laitteista?</span><span class="sxs-lookup"><span data-stu-id="b41b7-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="b41b7-114">: Intunen yrityssiitoittereiksi luokiteltuja puhelimia ei tunnisteta täydellä puhelinnumerolla, kun esimerkiksi suoritat mobiililaitteen inventaarioraportin.</span><span class="sxs-lookup"><span data-stu-id="b41b7-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="b41b7-115">Tuo sinulle oma-laite puhelinnumerot peitetään aina osittain tähtillä (\*\*\*\*), ja niissä näkyvät vain neljä viimeistä numeroa.</span><span class="sxs-lookup"><span data-stu-id="b41b7-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>