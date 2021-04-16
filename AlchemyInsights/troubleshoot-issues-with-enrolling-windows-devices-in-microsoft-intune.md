---
title: Windows-laitteiden microsoft Intunen rekisteröintiongelmien vianmääritys
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808968"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="7a9ef-102">Windows-laitteiden microsoft Intunen rekisteröintiongelmien vianmääritys</span><span class="sxs-lookup"><span data-stu-id="7a9ef-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="7a9ef-103">Ratkaise ongelma nyt alla lueteltujen resurssien avulla.</span><span class="sxs-lookup"><span data-stu-id="7a9ef-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="7a9ef-104">Yleisiä virhesanomia ja ratkaisuvaiheita:</span><span class="sxs-lookup"><span data-stu-id="7a9ef-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="7a9ef-105">**Ohjelmistoa ei voi asentaa, 0x80cf4017:** Tilivarmenne on vanhentunut.</span><span class="sxs-lookup"><span data-stu-id="7a9ef-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="7a9ef-106">Lataa PC-asiakasohjelman ohjelmistopaketti uudelleen Intune-hallintakonsolissa.</span><span class="sxs-lookup"><span data-stu-id="7a9ef-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="7a9ef-107">Katso lisätietoja tästä ohjeista.</span><span class="sxs-lookup"><span data-stu-id="7a9ef-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="7a9ef-108">**Virhekoodin 0x801c0003:** Virhe voi ilmetä seuraavissa tilanteissa:</span><span class="sxs-lookup"><span data-stu-id="7a9ef-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="7a9ef-109">Käyttäjällä on laiterajoitusta suurempia laitteita.</span><span class="sxs-lookup"><span data-stu-id="7a9ef-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="7a9ef-110">Tarkista nämä [asiakirjat, jos haluat poistaa laitteen](https://docs.microsoft.com/intune/devices-wipe) tai muuttaa laitteen [rajoitusta.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="7a9ef-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="7a9ef-111">Käyttäjät voivat liittyä laitteisiin Azure AD:ssä -asetuksena on Ei mitään.</span><span class="sxs-lookup"><span data-stu-id="7a9ef-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="7a9ef-112">Määritä se kaikille tai valitse käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="7a9ef-112">Set it to all or select users.</span></span> <span data-ttu-id="7a9ef-113">Katso [lisätietoja tästä](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) ohjeista.</span><span class="sxs-lookup"><span data-stu-id="7a9ef-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="7a9ef-114">Toinen käyttäjä on jo rekisteröinyt laitteen.</span><span class="sxs-lookup"><span data-stu-id="7a9ef-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="7a9ef-115">Poista tällöin laite Azure Intune -konsolista tai poista laitteen tilaus manuaalisesti ennen uudelleen yrittämistä.</span><span class="sxs-lookup"><span data-stu-id="7a9ef-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="7a9ef-116">Laite on Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="7a9ef-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="7a9ef-117">Vain Windows 10 Pro-, Education- ja Enterprise-SKU:t voivat liittyä Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="7a9ef-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="7a9ef-118">Lisäresursseja ongelman ratkaisemiseksi:</span><span class="sxs-lookup"><span data-stu-id="7a9ef-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="7a9ef-119">[Intunen vianmääritysportaalin avulla voit](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) tehdä vianmäärityksen ja ratkaista yleisiä rekisteröintivirheitä.</span><span class="sxs-lookup"><span data-stu-id="7a9ef-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="7a9ef-120">Katso [lisätietoja](https://docs.microsoft.com/intune/help-desk-operators) tästä asiakirjasta.</span><span class="sxs-lookup"><span data-stu-id="7a9ef-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="7a9ef-121">Tarkistamalla nämä asiakirjat saat luettelon yleisistä virheistä, jotka estävät kunkin tiedoston rekisteröinnin ja ratkaisut: [Vianmääritysopas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ja [Tiedoston vianmääritys.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="7a9ef-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="7a9ef-122">[Lue, miten voit rekisteröidä Windows-laitteita Microsoft Intunessa.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="7a9ef-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
