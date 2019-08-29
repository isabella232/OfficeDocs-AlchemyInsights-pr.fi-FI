---
title: Windows-laitteiden ilmoittautumalla-ongelmien vian määritys Microsoft Intunessa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665829"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="31aa4-102">Windows-laitteiden ilmoittautumalla-ongelmien vian määritys Microsoft Intunessa</span><span class="sxs-lookup"><span data-stu-id="31aa4-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="31aa4-103">Tarkista alla luetellut resurssit ongelman ratkaisemiseksi nyt.</span><span class="sxs-lookup"><span data-stu-id="31aa4-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="31aa4-104">Yleisiä virhe sanomia ja ratkaisu vaiheita:</span><span class="sxs-lookup"><span data-stu-id="31aa4-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="31aa4-105">**Ohjelmistoa ei voi asentaa, 0x80cf4017:** Tilisi varmenne on vanhentunut.</span><span class="sxs-lookup"><span data-stu-id="31aa4-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="31aa4-106">Lataa PC-asiakas ohjelmisto paketti uudelleen Intune admin Consolessa.</span><span class="sxs-lookup"><span data-stu-id="31aa4-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="31aa4-107">Saat lisä tietoja tästä dokumentaatiosta.</span><span class="sxs-lookup"><span data-stu-id="31aa4-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="31aa4-108">**Virhe koodi 0x801c0003:** Virhe voi ilmetä seuraavissa tilanteissa:</span><span class="sxs-lookup"><span data-stu-id="31aa4-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="31aa4-109">Käyttäjällä on enemmän laitteita, jotka on rekisteröity kuin laitteen rajoitus.</span><span class="sxs-lookup"><span data-stu-id="31aa4-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="31aa4-110">Voit [poistaa laitteen](https://docs.microsoft.com/intune/devices-wipe) tai [muuttaa laitteen rajaa](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)näiden asia kirjojen avulla.</span><span class="sxs-lookup"><span data-stu-id="31aa4-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="31aa4-111">"Käyttäjät voivat liittyä laitteisiin Azure AD"-arvoksi on määritetty "ei mitään".</span><span class="sxs-lookup"><span data-stu-id="31aa4-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="31aa4-112">Aseta se kaikille tai valitse käyttäjät.</span><span class="sxs-lookup"><span data-stu-id="31aa4-112">Set it to all or select users.</span></span> <span data-ttu-id="31aa4-113">Saat lisä tietoja [tästä dokumentaatiosta](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="31aa4-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="31aa4-114">Toinen käyttäjä on jo rekisteröitynyt laitteeseen.</span><span class="sxs-lookup"><span data-stu-id="31aa4-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="31aa4-115">Jos näin on, Poista laite Azure Intune-konsolista tai rekisteröi laite manuaalisesti, ennen kuin yrität uudelleen.</span><span class="sxs-lookup"><span data-stu-id="31aa4-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="31aa4-116">Laite on Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="31aa4-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="31aa4-117">Vain Windows 10 Pro, koulutus ja yritys yksiköt voivat liittyä Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="31aa4-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="31aa4-118">Lisä resursseja ongelman ratkaisemiseen:</span><span class="sxs-lookup"><span data-stu-id="31aa4-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="31aa4-119">Käytä [Intune-vian määritys portaalia](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) yleisten rekisteröinti virheiden diagnosoimiseen ja ratkaisemiseen.</span><span class="sxs-lookup"><span data-stu-id="31aa4-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="31aa4-120">Lisä tietoja [on tämän asia kirjan](https://docs.microsoft.com/intune/help-desk-operators) tarkastelussa.</span><span class="sxs-lookup"><span data-stu-id="31aa4-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="31aa4-121">Tarkastele näitä asia kirjoja, joissa on luettelo yleisistä virheistä, jotka estävät rekisteröintiä ja resoluutioita kuhunkin: [vian määritys opas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ja [vian etsintä doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="31aa4-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="31aa4-122">[Lue, miten voit rekisteröidä Windows-laitteita Microsoft Intune-kohteessa](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="31aa4-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
