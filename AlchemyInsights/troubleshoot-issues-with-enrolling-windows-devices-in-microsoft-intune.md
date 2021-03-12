---
title: Windows-laitteiden rekisteröintiongelmien vianmääritys Microsoft Intunessa
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
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708887"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="50a5f-102">Windows-laitteiden rekisteröintiongelmien vianmääritys Microsoft Intunessa</span><span class="sxs-lookup"><span data-stu-id="50a5f-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="50a5f-103">Ratkaise ongelmasi nyt alla lueteltujen resurssien avulla.</span><span class="sxs-lookup"><span data-stu-id="50a5f-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="50a5f-104">Joitakin yleisiä virhesanomia ja ratkaisuvaiheita:</span><span class="sxs-lookup"><span data-stu-id="50a5f-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="50a5f-105">**Ohjelmistoa ei voi asentaa, 0x80cf4017:** Tilivarmenne on vanhentunut.</span><span class="sxs-lookup"><span data-stu-id="50a5f-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="50a5f-106">Lataa PC Client -ohjelmistopaketti uudelleen Intune-hallintakonsolissa.</span><span class="sxs-lookup"><span data-stu-id="50a5f-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="50a5f-107">Saat lisätietoja tästä ohjeista.</span><span class="sxs-lookup"><span data-stu-id="50a5f-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="50a5f-108">**Virhekoodin 0x801c0003:** Virhe voi ilmetä seuraavissa tilanteissa:</span><span class="sxs-lookup"><span data-stu-id="50a5f-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="50a5f-109">Käyttäjällä on enemmän laitteita, jotka on rekisteröity laiterajoitusta enemmän.</span><span class="sxs-lookup"><span data-stu-id="50a5f-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="50a5f-110">Voit poistaa laitteen [tai muuttaa laiterajoitusta](https://docs.microsoft.com/intune/devices-wipe) [tarkistamalla nämä asiakirjat.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="50a5f-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="50a5f-111">Käyttäjät voivat liittyä laitteisiin Azure AD:ssä -asetuksena on Ei mitään.</span><span class="sxs-lookup"><span data-stu-id="50a5f-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="50a5f-112">Määritä se kaikille tai valitse käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="50a5f-112">Set it to all or select users.</span></span> <span data-ttu-id="50a5f-113">Saat [lisätietoja tästä](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) ohjeista.</span><span class="sxs-lookup"><span data-stu-id="50a5f-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="50a5f-114">Toinen käyttäjä on jo rekisteröinyt laitteen.</span><span class="sxs-lookup"><span data-stu-id="50a5f-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="50a5f-115">Jos näin on, poista laite Azure Intune -konsolista tai poista laitteen tilaus manuaalisesti, ennen kuin yrität uudelleen.</span><span class="sxs-lookup"><span data-stu-id="50a5f-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="50a5f-116">Laite on Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="50a5f-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="50a5f-117">Vain Windows 10 Pro-, Education- ja Enterprise-käyttäjät voivat liittyä Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="50a5f-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="50a5f-118">Lisäresursseja ongelman ratkaisemiseen:</span><span class="sxs-lookup"><span data-stu-id="50a5f-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="50a5f-119">[Intunen vianmääritysportaalin avulla](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) voit diagnosoida ja ratkaista yleisiä rekisteröintivirheitä.</span><span class="sxs-lookup"><span data-stu-id="50a5f-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="50a5f-120">Katso [lisätietoja tästä](https://docs.microsoft.com/intune/help-desk-operators) asiakirjasta.</span><span class="sxs-lookup"><span data-stu-id="50a5f-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="50a5f-121">Tarkistamalla nämä asiakirjat saat luettelon yleisistä virheistä, jotka estävät rekisteröitymisen ja ratkaisut kuhunkin: [vianmääritysopas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ja [vianmäärityksen asiakirja.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="50a5f-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="50a5f-122">[Opi rekisteröimaan Windows-laitteita Microsoft Intunessa.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="50a5f-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
