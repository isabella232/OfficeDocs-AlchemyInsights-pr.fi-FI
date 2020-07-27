---
title: Ohita aktivointilukitus valvotuissa iOS-laitteissa Intunen avulla
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423735"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="f1852-102">Ohita aktivointilukitus valvotuissa iOS-laitteissa Intunen avulla</span><span class="sxs-lookup"><span data-stu-id="f1852-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="f1852-103">IOS-laitteiden aktivointilukituksen ohittaminen helpottaa toipumista skenaariosta, jossa käyttäjä ottaa käyttöön aktivointilukituksen yrityslaitteessa ja poistuu sitten yrityksestä.</span><span class="sxs-lookup"><span data-stu-id="f1852-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="f1852-104">Aktivointilukon ohittamisen edellytyksenä ovat seuraavat:</span><span class="sxs-lookup"><span data-stu-id="f1852-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="f1852-105">Laite on "valvottu".</span><span class="sxs-lookup"><span data-stu-id="f1852-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="f1852-106">Aktivointilukitus on otettu käyttöön iOS-laiterajoituskäytännön avulla Intuessa.</span><span class="sxs-lookup"><span data-stu-id="f1852-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="f1852-107">Lisäksi aktivointilukon ohitettaessa sinun on</span><span class="sxs-lookup"><span data-stu-id="f1852-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="f1852-108">Fyysisesti hallussaan laite pyyhitään.</span><span class="sxs-lookup"><span data-stu-id="f1852-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="f1852-109">Kopioi koodi ennen pyyhkimisen antamista.</span><span class="sxs-lookup"><span data-stu-id="f1852-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="f1852-110">**Huomautus:** Pyyhikoodissa isot ja pienet kirjaimet eivät ole isot ja pienet kirjaimet, joten "-"-merkkejä ei tarvita.</span><span class="sxs-lookup"><span data-stu-id="f1852-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="f1852-111">Lisätietoja on kohdassa [Aktivointilukituksen ohitttaminen valvotuissa iOS-laitteissa Intune -toiminnolla](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="f1852-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="f1852-112">**Usein kysytyt kysymykset**</span><span class="sxs-lookup"><span data-stu-id="f1852-112">**FAQ**</span></span>

<span data-ttu-id="f1852-113">K: **Tein etätoiminnon yrityksen tietojen poistamiseksi laitteesta, ja nyt se on jumissa odottavassa tilassa.**</span><span class="sxs-lookup"><span data-stu-id="f1852-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="f1852-114">: Jotta etätoiminto onnistuisi, kohdelaitteen on oltava online-tilassa ja terve.</span><span class="sxs-lookup"><span data-stu-id="f1852-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="f1852-115">Seuraavissa tilanteissa etätoiminto pysyy odottavassa tilassa 30 päivän ajan tai kunnes laite hyväksyy komennon, kun laite:</span><span class="sxs-lookup"><span data-stu-id="f1852-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="f1852-116">Ei ole yhteyttä.</span><span class="sxs-lookup"><span data-stu-id="f1852-116">Does not have connectivity.</span></span>
- <span data-ttu-id="f1852-117">Menettää johdon tilan Intunella.</span><span class="sxs-lookup"><span data-stu-id="f1852-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="f1852-118">Jos epäilet, että laite ei enää kirjaudu sisään ja että se ei poista yrityksen tietoja, valitse Poista.</span><span class="sxs-lookup"><span data-stu-id="f1852-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="f1852-119">Poistaminen poistaa laitetietueen niin, että se ei enää näy Intune-laiteluettelossa.</span><span class="sxs-lookup"><span data-stu-id="f1852-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="f1852-120">Jotta laite aktivoituu uudelleen, sen käyttäjän on rekisteröitävä laite uudelleen.</span><span class="sxs-lookup"><span data-stu-id="f1852-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="f1852-121">K: **Miksi tietyt etätoiminnot eivät ole käytettävissä?**</span><span class="sxs-lookup"><span data-stu-id="f1852-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="f1852-122">A: Kaikki alustat eivät tue kaikkia etälaitetoimintoja.</span><span class="sxs-lookup"><span data-stu-id="f1852-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="f1852-123">Seuraavat etätoiminnot ovat ympäristökohtaisia.</span><span class="sxs-lookup"><span data-stu-id="f1852-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="f1852-124">Ohita aktivointilukitus (vain iOS)</span><span class="sxs-lookup"><span data-stu-id="f1852-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="f1852-125">Tuore käynnistys (vain Windows)</span><span class="sxs-lookup"><span data-stu-id="f1852-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="f1852-126">Kadonnut-tila (vain iOS)</span><span class="sxs-lookup"><span data-stu-id="f1852-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="f1852-127">Laitteen paikantaminen (vain iOS)</span><span class="sxs-lookup"><span data-stu-id="f1852-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="f1852-128">Käynnistä uudelleen (vain Windows)</span><span class="sxs-lookup"><span data-stu-id="f1852-128">Restart (Windows only)</span></span>

<span data-ttu-id="f1852-129">Lisätietoja kustakin toiminnosta on kohdassa [Käytettävissä olevat laitetoiminnot](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="f1852-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>