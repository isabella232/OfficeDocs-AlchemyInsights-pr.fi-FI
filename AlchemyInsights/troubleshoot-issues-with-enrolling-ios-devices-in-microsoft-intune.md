---
title: Rekisteröiminen Microsoft Intune iOS-laitteiden ongelmien vianmääritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29924765"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="a7208-102">Rekisteröiminen Microsoft Intune iOS-laitteiden ongelmien vianmääritys</span><span class="sxs-lookup"><span data-stu-id="a7208-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="a7208-103">Tarkista ongelman nyt alla luetellut resurssit.</span><span class="sxs-lookup"><span data-stu-id="a7208-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="a7208-104">Joitakin yleisiä virhesanomia ja tarkkuutta vaiheet:</span><span class="sxs-lookup"><span data-stu-id="a7208-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="a7208-p101">**Laitteen Cap saavutettu** Käyttäjä on rekisteröitynyt ylittää laitteen enimmäiskoon laitteita. Tarkasteltava näitä asiakirjoja, voit [poistaa laitteen](https://docs.microsoft.com/intune/devices-wipe) tai [muuttaa laitteen enimmäiskoon](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="a7208-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="a7208-p102">**: Tämä palvelu ei tue. Rekisteröintikäytäntö ei:** Apple Push Notification Service (APNS) on määritetty tai uudistaa. Lue [tämän asiakirjan](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) ohjeita tämän tekemisestä.</span><span class="sxs-lookup"><span data-stu-id="a7208-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="a7208-p103">**Käyttäjän käyttöoikeuden tyyppi ei kelpaa tai käyttäjänimeä ei tunnisteta:** Käyttäjän on oltava Intune tai EMS-käyttöoikeus. Tarkasteltava näitä asiakirjoja käyttöoikeuden kautta: [Office Admin Centerissä](https://docs.microsoft.com/intune/licenses-assign) tai [Azure portaalin](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="a7208-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="a7208-111">Lisätietoja ja resursseja auttaa ratkaisemaan ongelmaasi:</span><span class="sxs-lookup"><span data-stu-id="a7208-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="a7208-p104">[Intune vianmääritys-portaalin](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) avulla voit diagnosoida ja ratkaista yhteisen rekisteröinti virheitä. Lisätietoja [tämän asiakirjan](https://docs.microsoft.com/intune/help-desk-operators) tarkasteleminen.</span><span class="sxs-lookup"><span data-stu-id="a7208-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="a7208-114">Tarkasteltava näitä asiakirjoja yleisiä virheitä, jotka estävät rekisteröinti ja ratkaisuja jokaiseen luettelo: [Vianetsintä opas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ja [vianmääritys doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="a7208-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="a7208-115">[Rekisteröi Microsoft Intune iOS-laitteiden tietoja](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="a7208-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

