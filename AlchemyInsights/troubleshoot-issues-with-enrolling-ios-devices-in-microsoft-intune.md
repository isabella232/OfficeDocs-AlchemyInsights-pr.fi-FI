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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391004"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="9cc03-102">Rekisteröiminen Microsoft Intune iOS-laitteiden ongelmien vianmääritys</span><span class="sxs-lookup"><span data-stu-id="9cc03-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="9cc03-103">Tarkista ongelman nyt alla luetellut resurssit.</span><span class="sxs-lookup"><span data-stu-id="9cc03-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="9cc03-104">Joitakin yleisiä virhesanomia ja tarkkuutta vaiheet:</span><span class="sxs-lookup"><span data-stu-id="9cc03-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="9cc03-105">**Laitteen Cap saavutettu** Käyttäjä on rekisteröitynyt ylittää laitteen enimmäiskoon laitteita.</span><span class="sxs-lookup"><span data-stu-id="9cc03-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="9cc03-106">Tarkasteltava näitä asiakirjoja, voit [poistaa laitteen](https://docs.microsoft.com/intune/devices-wipe) tai [muuttaa laitteen enimmäiskoon](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="9cc03-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="9cc03-107">**: Tämä palvelu ei tue. Rekisteröintikäytäntö ei:** Apple Push Notification Service (APNS) on määritetty tai uudistaa.</span><span class="sxs-lookup"><span data-stu-id="9cc03-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="9cc03-108">Lue [tämän asiakirjan](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) ohjeita tämän tekemisestä.</span><span class="sxs-lookup"><span data-stu-id="9cc03-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="9cc03-109">**Käyttäjän käyttöoikeuden tyyppi ei kelpaa tai käyttäjänimeä ei tunnisteta:** Käyttäjän on oltava Intune tai EMS-käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="9cc03-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="9cc03-110">Tarkasteltava näitä asiakirjoja käyttöoikeuden kautta: [Office Admin Centerissä](https://docs.microsoft.com/intune/licenses-assign) tai [Azure portaalin](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="9cc03-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="9cc03-111">Lisätietoja ja resursseja auttaa ratkaisemaan ongelmaasi:</span><span class="sxs-lookup"><span data-stu-id="9cc03-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="9cc03-112">[Intune vianmääritys-portaalin](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) avulla voit diagnosoida ja ratkaista yhteisen rekisteröinti virheitä.</span><span class="sxs-lookup"><span data-stu-id="9cc03-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="9cc03-113">Lisätietoja [tämän asiakirjan](https://docs.microsoft.com/intune/help-desk-operators) tarkasteleminen.</span><span class="sxs-lookup"><span data-stu-id="9cc03-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="9cc03-114">Tarkasteltava näitä asiakirjoja yleisiä virheitä, jotka estävät rekisteröinti ja ratkaisuja jokaiseen luettelo: [Vianetsintä opas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ja [vianmääritys doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="9cc03-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="9cc03-115">[Rekisteröi Microsoft Intune iOS-laitteiden tietoja](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="9cc03-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

