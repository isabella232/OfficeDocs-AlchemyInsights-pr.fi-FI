---
title: iOS-laitteiden rekisteröintiongelmien vianmääritys Microsoft Intunessa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708959"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="e181f-102">iOS-laitteiden rekisteröintiongelmien vianmääritys Microsoft Intunessa</span><span class="sxs-lookup"><span data-stu-id="e181f-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="e181f-103">Ratkaise ongelmasi nyt alla lueteltujen resurssien avulla.</span><span class="sxs-lookup"><span data-stu-id="e181f-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="e181f-104">Joitakin yleisiä virhesanomia ja ratkaisuvaiheita:</span><span class="sxs-lookup"><span data-stu-id="e181f-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="e181f-105">**Laitteen kapi on saavutettu** Käyttäjällä on enemmän laitteita, jotka on rekisteröity laiterajoitusta enemmän.</span><span class="sxs-lookup"><span data-stu-id="e181f-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="e181f-106">Voit poistaa laitteen [tai muuttaa laiterajoitusta](https://docs.microsoft.com/intune/devices-wipe) [tarkistamalla nämä asiakirjat.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="e181f-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="e181f-107">**Tätä palvelua ei tueta. Ei rekisteröintikäytäntöä:** Apple Push Notification Service (APNS) on määritettävä tai uusittava.</span><span class="sxs-lookup"><span data-stu-id="e181f-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="e181f-108">Katso [ohjeet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) tähän asiakirjaan.</span><span class="sxs-lookup"><span data-stu-id="e181f-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="e181f-109">**Käyttäjäkäyttöoikeustyyppi virheellinen tai käyttäjänimiä ei tunnisteta:** Käyttäjälle on oltava määritetty Intune- tai EMS-käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="e181f-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="e181f-110">Tarkista nämä asiakirjat ja määritä käyttöoikeus Office-hallintakeskuksen tai [Azure-portaalin kautta.](https://docs.microsoft.com/azure/active-directory/license-users-groups) [](https://docs.microsoft.com/intune/licenses-assign)</span><span class="sxs-lookup"><span data-stu-id="e181f-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="e181f-111">Lisäresursseja ongelman ratkaisemiseen:</span><span class="sxs-lookup"><span data-stu-id="e181f-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="e181f-112">[Intunen vianmääritysportaalin avulla](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) voit diagnosoida ja ratkaista yleisiä rekisteröintivirheitä.</span><span class="sxs-lookup"><span data-stu-id="e181f-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="e181f-113">Katso [lisätietoja tästä](https://docs.microsoft.com/intune/help-desk-operators) asiakirjasta.</span><span class="sxs-lookup"><span data-stu-id="e181f-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="e181f-114">Tarkistamalla nämä asiakirjat saat luettelon yleisistä virheistä, jotka estävät rekisteröitymisen ja ratkaisut kuhunkin: [vianmääritysopas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ja [vianmäärityksen asiakirja.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="e181f-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="e181f-115">[Lue, miten voit rekisteröidä iOS-laitteita Microsoft Intunessa.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="e181f-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

