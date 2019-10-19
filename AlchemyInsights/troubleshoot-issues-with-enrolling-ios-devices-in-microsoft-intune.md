---
title: IOS-laitteiden ilmoittautumalla-ongelmien vian määritys Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36506922"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="19de1-102">IOS-laitteiden ilmoittautumalla-ongelmien vian määritys Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="19de1-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="19de1-103">Tarkista alla luetellut resurssit ongelman ratkaisemiseksi nyt.</span><span class="sxs-lookup"><span data-stu-id="19de1-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="19de1-104">Yleisiä virhe sanomia ja ratkaisu vaiheita:</span><span class="sxs-lookup"><span data-stu-id="19de1-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="19de1-105">**Laitteen suojus saavutettu** Käyttäjällä on enemmän laitteita, jotka on rekisteröity kuin laitteen rajoitus.</span><span class="sxs-lookup"><span data-stu-id="19de1-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="19de1-106">Voit [poistaa laitteen](https://docs.microsoft.com/intune/devices-wipe) tai [muuttaa laitteen rajaa](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)näiden asia kirjojen avulla.</span><span class="sxs-lookup"><span data-stu-id="19de1-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="19de1-107">**Tätä palvelua ei tueta. Ei rekisteröinti käytäntöä:** Applen push-ilmoitus palvelu (APNS) on määritettävä tai uusittava.</span><span class="sxs-lookup"><span data-stu-id="19de1-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="19de1-108">Tarkastele [tätä asia kirjaa](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , niin saat ohjeita.</span><span class="sxs-lookup"><span data-stu-id="19de1-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="19de1-109">**Käyttö oikeus tyyppi ei kelpaa, tai käyttäjä nimeä ei tunnistettu:** Käyttäjälle on määritettävä Intune-tai EMS-lisenssi.</span><span class="sxs-lookup"><span data-stu-id="19de1-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="19de1-110">Voit määrittää käyttö oikeuden näiden asia kirjojen avulla [Office-hallinta keskukseen](https://docs.microsoft.com/intune/licenses-assign) tai [Azure-portaaliin](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="19de1-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="19de1-111">Lisä resursseja ongelman ratkaisemiseen:</span><span class="sxs-lookup"><span data-stu-id="19de1-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="19de1-112">Käytä [Intune-vian määritys portaalia](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) yleisten rekisteröinti virheiden diagnosoimiseen ja ratkaisemiseen.</span><span class="sxs-lookup"><span data-stu-id="19de1-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="19de1-113">Lisä tietoja [on tämän asia kirjan](https://docs.microsoft.com/intune/help-desk-operators) tarkastelussa.</span><span class="sxs-lookup"><span data-stu-id="19de1-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="19de1-114">Tarkastele näitä asia kirjoja, joissa on luettelo yleisistä virheistä, jotka estävät rekisteröintiä ja resoluutioita kuhunkin: [vian määritys opas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ja [vian etsintä doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="19de1-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="19de1-115">[Lue, miten voit rekisteröidä iOS-laitteita Microsoft Intunessa](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="19de1-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

