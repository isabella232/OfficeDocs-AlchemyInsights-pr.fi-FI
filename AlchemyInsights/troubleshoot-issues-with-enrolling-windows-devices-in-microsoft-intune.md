---
title: Windows-laitteiden rekisteröimiseen Microsoft Intuneen liittyvien ongelmien vianmääritys
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
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665829"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="9859f-102">Windows-laitteiden rekisteröimiseen Microsoft Intuneen liittyvien ongelmien vianmääritys</span><span class="sxs-lookup"><span data-stu-id="9859f-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="9859f-103">Tarkastele alla lueteltuja resursseja ratkaistaksesi ongelman nyt.</span><span class="sxs-lookup"><span data-stu-id="9859f-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="9859f-104">Joitakin yleisiä virhesanomia ja ratkaisuvaiheita:</span><span class="sxs-lookup"><span data-stu-id="9859f-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="9859f-105">**Ohjelmistoa ei voi asentaa, 0x80cf4017:** Tilisi varmenne on vanhentunut.</span><span class="sxs-lookup"><span data-stu-id="9859f-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="9859f-106">Lataa PC Client -ohjelmistopaketti uudelleen Intune Admin Consolessa.</span><span class="sxs-lookup"><span data-stu-id="9859f-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="9859f-107">Lisätietoja on näissä ohjeissa.</span><span class="sxs-lookup"><span data-stu-id="9859f-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="9859f-108">**Virhekoodi 0x801c0003:** Virhe voi ilmetä seuraavissa tilanteissa:</span><span class="sxs-lookup"><span data-stu-id="9859f-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="9859f-109">Käyttäjällä on enemmän laitteita, jotka on rekisteröity laiterajaa suuremmaksi.</span><span class="sxs-lookup"><span data-stu-id="9859f-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="9859f-110">Näiden asiakirjojen avulla voit [poistaa laitteen](https://docs.microsoft.com/intune/devices-wipe) tai [muuttaa laiterajoitusta](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="9859f-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="9859f-111">"Käyttäjät voivat liittyä laitteisiin Azure AD:hen" -asetuksena on ei mitään.</span><span class="sxs-lookup"><span data-stu-id="9859f-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="9859f-112">Aseta se kaikille tai valitse käyttäjät.</span><span class="sxs-lookup"><span data-stu-id="9859f-112">Set it to all or select users.</span></span> <span data-ttu-id="9859f-113">Lisätietoja [on näissä ohjeissa.](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)</span><span class="sxs-lookup"><span data-stu-id="9859f-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="9859f-114">Toinen käyttäjä on jo rekisteröinyt laitteen.</span><span class="sxs-lookup"><span data-stu-id="9859f-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="9859f-115">Jos näin on, poista laite Azure Intune -konsolista tai poista laite manuaalisesti käytöstä ennen kuin yrität uudelleen.</span><span class="sxs-lookup"><span data-stu-id="9859f-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="9859f-116">Laite on Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="9859f-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="9859f-117">Azure Active Directoryyn voi liittyä vain Windows 10 Pro-, Education- ja Enterprise SKU -käyttöyksiköt.</span><span class="sxs-lookup"><span data-stu-id="9859f-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="9859f-118">Muita resursseja ongelman ratkaisemiseen:</span><span class="sxs-lookup"><span data-stu-id="9859f-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="9859f-119">[Intune Troubleshooting Portalin](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) avulla voit diagnosoida ja ratkaista yleisiä rekisteröintivirheitä.</span><span class="sxs-lookup"><span data-stu-id="9859f-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="9859f-120">Lisätietoja on [tässä asiakirjassa.](https://docs.microsoft.com/intune/help-desk-operators)</span><span class="sxs-lookup"><span data-stu-id="9859f-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="9859f-121">Näiden asiakirjojen on luettelo yleisistä virheistä, jotka estävät rekisteröitymisen ja ratkaisut kuhunkin: [Vianmääritysopas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ja [Vianmääritys-asiakirja](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="9859f-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="9859f-122">[Tietoja Windows-laitteiden rekisteröimisestä Microsoft Intutiin.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="9859f-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
