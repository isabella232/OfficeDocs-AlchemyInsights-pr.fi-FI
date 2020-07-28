---
title: Kadonneiden iOS-laitteiden etsiminen Intunen avulla
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
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439625"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="b41e5-102">Kadonneiden iOS-laitteiden etsiminen Intunen avulla</span><span class="sxs-lookup"><span data-stu-id="b41e5-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="b41e5-103">Kun kadonnut tila otetaan käyttöön iOS-laitteessa, järjestelmänvalvoja voi näyttää lukitusnäytössä viestin ja puhelinnumeron.</span><span class="sxs-lookup"><span data-stu-id="b41e5-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="b41e5-104">Kun kadonnut tila on käytössä, järjestelmänvalvoja voi paikantaa laitteen paikannuksen avulla laitteen fyysisen sijainnin.</span><span class="sxs-lookup"><span data-stu-id="b41e5-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="b41e5-105">Intunen Paikanna laite -toiminto toimii iOS-laitteiden kanssa näyttääkseen tietyn laitteen sijainnin kartalla.</span><span class="sxs-lookup"><span data-stu-id="b41e5-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="b41e5-106">Tämän toiminnon käyttäminen edellyttää, että iOS-laite on:</span><span class="sxs-lookup"><span data-stu-id="b41e5-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="b41e5-107">Valvottu tila</span><span class="sxs-lookup"><span data-stu-id="b41e5-107">Supervised mode</span></span>
- <span data-ttu-id="b41e5-108">Kadonnut-tila</span><span class="sxs-lookup"><span data-stu-id="b41e5-108">Lost mode</span></span>

<span data-ttu-id="b41e5-109">Lisätietoja on ohjeissa [Kadonneen tilan ottaminen käyttöön iOS/iPadOS-laitteissa, joissa on Intune](https://docs.microsoft.com/intune/device-lost-mode) ja [Etsi kadonneet tai varastetut iOS/iPadOS-laitteet Intunella](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="b41e5-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="b41e5-110">**Usein kysytyt kysymykset**</span><span class="sxs-lookup"><span data-stu-id="b41e5-110">**FAQ**</span></span>

<span data-ttu-id="b41e5-111">K: Tein etätoiminnon yrityksen tietojen poistamiseksi laitteesta, ja nyt se on jumissa odottavassa tilassa.</span><span class="sxs-lookup"><span data-stu-id="b41e5-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="b41e5-112">: Jotta etätoiminto onnistuisi, kohdelaitteen on oltava online-tilassa ja terve.</span><span class="sxs-lookup"><span data-stu-id="b41e5-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="b41e5-113">Seuraavissa tilanteissa etätoiminto pysyy odottavassa tilassa 30 päivän ajan tai kunnes laite hyväksyy komennon:</span><span class="sxs-lookup"><span data-stu-id="b41e5-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="b41e5-114">Jos laitteessa ei ole yhteyttä</span><span class="sxs-lookup"><span data-stu-id="b41e5-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="b41e5-115">Kun laite menettää hallintatilansa Intune</span><span class="sxs-lookup"><span data-stu-id="b41e5-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="b41e5-116">Jos epäilet, että laite ei enää kirjaudu sisään ja että se ei voi poistaa yrityksen tietoja, valitse Poista.</span><span class="sxs-lookup"><span data-stu-id="b41e5-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="b41e5-117">Poistaminen poistaa laitetietueen niin, että se ei enää näy Intune-laiteluettelossa.</span><span class="sxs-lookup"><span data-stu-id="b41e5-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="b41e5-118">Jos laite aktivoituu uudelleen, sen käyttäjän on rekisteröitävä se uudelleen.</span><span class="sxs-lookup"><span data-stu-id="b41e5-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="b41e5-119">K: Miksi tietyt etätoiminnot eivät ole käytettävissä?</span><span class="sxs-lookup"><span data-stu-id="b41e5-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="b41e5-120">A: Kaikki alustat eivät tue kaikkia etälaitetoimintoja.</span><span class="sxs-lookup"><span data-stu-id="b41e5-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="b41e5-121">Seuraavat etätoiminnot ovat alustakohtaisia, joten ne ovat käytettävissä vain mainittujen alustojen osalta.</span><span class="sxs-lookup"><span data-stu-id="b41e5-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="b41e5-122">Ohita aktivointilukitus (vain iOS)</span><span class="sxs-lookup"><span data-stu-id="b41e5-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="b41e5-123">Tuore käynnistys (vain Windows)</span><span class="sxs-lookup"><span data-stu-id="b41e5-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="b41e5-124">Kadonnut-tila (vain iOS)</span><span class="sxs-lookup"><span data-stu-id="b41e5-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="b41e5-125">Laitteen paikantaminen (vain iOS)</span><span class="sxs-lookup"><span data-stu-id="b41e5-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="b41e5-126">Käynnistä uudelleen (vain Windows)</span><span class="sxs-lookup"><span data-stu-id="b41e5-126">Restart (Windows only)</span></span>

<span data-ttu-id="b41e5-127">Lisätietoja kustakin toiminnosta on kohdassa [Käytettävissä olevat laitetoiminnot](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="b41e5-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>