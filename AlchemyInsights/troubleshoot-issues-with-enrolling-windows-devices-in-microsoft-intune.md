---
title: Windows-laitteiden rekisteröimisen ongelmien vian määritys Microsoft Intunella
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658875"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="a8ceb-102">Windows-laitteiden rekisteröimisen ongelmien vian määritys Microsoft Intunella</span><span class="sxs-lookup"><span data-stu-id="a8ceb-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="a8ceb-103">Ratkaise ongelma nyt alla lueteltujen resurssien avulla.</span><span class="sxs-lookup"><span data-stu-id="a8ceb-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="a8ceb-104">Yleisiä virhe sanomia ja ratkaisu vaiheita:</span><span class="sxs-lookup"><span data-stu-id="a8ceb-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="a8ceb-105">**Ohjelmistoa ei voi asentaa, 0x80cf4017:** Tili varmenne on vanhentunut.</span><span class="sxs-lookup"><span data-stu-id="a8ceb-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="a8ceb-106">Lataa uudelleen PC-asiakas ohjelmisto paketti Intune-hallinta konsolissa.</span><span class="sxs-lookup"><span data-stu-id="a8ceb-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="a8ceb-107">Katso lisä tietoja tästä dokumentaatiosta.</span><span class="sxs-lookup"><span data-stu-id="a8ceb-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="a8ceb-108">**Virhe koodi 0x801c0003:** Virhe voi ilmetä seuraavissa tilanteissa:</span><span class="sxs-lookup"><span data-stu-id="a8ceb-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="a8ceb-109">Käyttäjällä on enemmän laitteita, jotka ovat rekisteröityneet kuin laitteen raja.</span><span class="sxs-lookup"><span data-stu-id="a8ceb-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="a8ceb-110">Tarkista nämä asia kirjat, jos haluat [poistaa laitteen](https://docs.microsoft.com/intune/devices-wipe) tai [muuttaa laitteen rajoitusta](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="a8ceb-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="a8ceb-111">"Käyttäjät voivat liittyä laitteisiin Azure AD:hen"-asetuksena on "ei mitään".</span><span class="sxs-lookup"><span data-stu-id="a8ceb-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="a8ceb-112">Määritä se kaikille tai valitse käyttäjät.</span><span class="sxs-lookup"><span data-stu-id="a8ceb-112">Set it to all or select users.</span></span> <span data-ttu-id="a8ceb-113">Katso lisä tietoja [tästä dokumentaatiosta](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="a8ceb-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="a8ceb-114">Toinen käyttäjä on jo rekisteröinyt laitteen.</span><span class="sxs-lookup"><span data-stu-id="a8ceb-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="a8ceb-115">Jos näin on, Poista laite Azure Intune-konsolista tai rekisteröi laite manuaalisesti, ennen kuin yrität uudelleen.</span><span class="sxs-lookup"><span data-stu-id="a8ceb-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="a8ceb-116">Laite on Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="a8ceb-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="a8ceb-117">Vain Windows 10 Pro, Education ja Enterprise SKUs voivat liittyä Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="a8ceb-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="a8ceb-118">Lisä resursseja ongelman ratkaisemiseen:</span><span class="sxs-lookup"><span data-stu-id="a8ceb-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="a8ceb-119">Käytä [Intune-vian määritys portaalia](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) yleisten rekisteröinti virheiden diagnosointiin ja ratkaisemiseen.</span><span class="sxs-lookup"><span data-stu-id="a8ceb-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="a8ceb-120">Katso lisä tietoja [tästä asia kirjasta](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="a8ceb-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="a8ceb-121">Tutustu näihin asia kirjoihin, jos haluat luettelon yleisistä virheistä, jotka estävät rekisteröinnin ja päätös lauselmien kunkin: [vian määritys opas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ja [vian määritys-asiak](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="a8ceb-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="a8ceb-122">[Opi rekisteröimään Windows-laitteet Microsoft Intunella](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="a8ceb-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
