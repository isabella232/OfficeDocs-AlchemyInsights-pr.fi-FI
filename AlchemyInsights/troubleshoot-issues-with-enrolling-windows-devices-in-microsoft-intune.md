---
title: Rekisteröiminen Windows Microsoft Intune-laitteiden ongelmien vianmääritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: fa48b76fb49cdeef0734e77520c9bf95c150f317
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353534"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="b77e9-102">Rekisteröiminen Windows Microsoft Intune-laitteiden ongelmien vianmääritys</span><span class="sxs-lookup"><span data-stu-id="b77e9-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="b77e9-103">Tarkista ongelman nyt alla luetellut resurssit.</span><span class="sxs-lookup"><span data-stu-id="b77e9-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="b77e9-104">Joitakin yleisiä virhesanomia ja tarkkuutta vaiheet:</span><span class="sxs-lookup"><span data-stu-id="b77e9-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="b77e9-105">**Ei voi asentaa ohjelmiston 0x80cf4017:** Käyttäjän tili on vanhentunut.</span><span class="sxs-lookup"><span data-stu-id="b77e9-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="b77e9-106">Lataa uudelleen PC-Client-ohjelmistopaketin Intune hallintakonsolissa.</span><span class="sxs-lookup"><span data-stu-id="b77e9-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="b77e9-107">Tarkista tästä lisätietoja ohjeista.</span><span class="sxs-lookup"><span data-stu-id="b77e9-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="b77e9-108">**0x801c0003-virhekoodi:** Virhe voi ilmetä seuraavissa tilanteissa:</span><span class="sxs-lookup"><span data-stu-id="b77e9-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
1. <span data-ttu-id="b77e9-109">Käyttäjä on rekisteröitynyt ylittää laitteen enimmäiskoon laitteita.</span><span class="sxs-lookup"><span data-stu-id="b77e9-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="b77e9-110">Tarkasteltava näitä asiakirjoja, voit [poistaa laitteen](https://docs.microsoft.com/intune/devices-wipe) tai [muuttaa laitteen enimmäiskoon](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="b77e9-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

2. <span data-ttu-id="b77e9-111">”Käyttäjät voivat liittää laitteet Azure AD” on määritetty ”none”.</span><span class="sxs-lookup"><span data-stu-id="b77e9-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="b77e9-112">Valitse tai määritä se kaikille käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="b77e9-112">Set it to all or select users.</span></span> <span data-ttu-id="b77e9-113">Voit tarkastella [näitä ohjeita](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="b77e9-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

3. <span data-ttu-id="b77e9-114">Toinen käyttäjä on jo liitetty laite.</span><span class="sxs-lookup"><span data-stu-id="b77e9-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="b77e9-115">Jos näin on, poista laite Azure Intune konsolista tai Peruuta laitteen ilmoittautuminen manuaalisesti ennen kuin yrität uudelleen.</span><span class="sxs-lookup"><span data-stu-id="b77e9-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

4. <span data-ttu-id="b77e9-116">Laite on Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="b77e9-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="b77e9-117">Vain Windows 10 Pro, koulutus ja Enterprise SKU-tietoja voit liittää Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b77e9-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="b77e9-118">Lisätietoja ja resursseja auttaa ratkaisemaan ongelmaasi:</span><span class="sxs-lookup"><span data-stu-id="b77e9-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="b77e9-119">[Intune vianmääritys-portaalin](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) avulla voit diagnosoida ja ratkaista yhteisen rekisteröinti virheitä.</span><span class="sxs-lookup"><span data-stu-id="b77e9-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="b77e9-120">Lisätietoja [tämän asiakirjan](https://docs.microsoft.com/intune/help-desk-operators) tarkasteleminen.</span><span class="sxs-lookup"><span data-stu-id="b77e9-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="b77e9-121">Tarkasteltava näitä asiakirjoja yleisiä virheitä, jotka estävät rekisteröinti ja ratkaisuja jokaiseen luettelo: [Vianetsintä opas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ja [vianmääritys doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="b77e9-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="b77e9-122">[Rekisteröi Windows Microsoft Intune-laitteiden tietoja](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="b77e9-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
