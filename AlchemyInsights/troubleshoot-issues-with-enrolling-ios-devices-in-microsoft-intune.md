---
title: iOS-laitteiden rekisteröiminen Microsoft Intunen ongelmien vianmääritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736155"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="9ce99-102">iOS-laitteiden rekisteröiminen Microsoft Intunen ongelmien vianmääritys</span><span class="sxs-lookup"><span data-stu-id="9ce99-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="9ce99-103">Ratkaise ongelma nyt alla olevien resurssien avulla.</span><span class="sxs-lookup"><span data-stu-id="9ce99-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="9ce99-104">Joitakin yleisiä virhesanomia ja ratkaisuvaiheita:</span><span class="sxs-lookup"><span data-stu-id="9ce99-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="9ce99-105">**Laitteen korkki saavutettu** Käyttäjällä on enemmän laitteita kuin laiteraja.</span><span class="sxs-lookup"><span data-stu-id="9ce99-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="9ce99-106">Poista [laite](https://docs.microsoft.com/intune/devices-wipe) tai muuta [laitteen rajaa](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)tarkastelemalla näitä asiakirjoja.</span><span class="sxs-lookup"><span data-stu-id="9ce99-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="9ce99-107">**Tätä palvelua ei tueta. Ei ilmoittautumiskäytäntöä:** Applen push-ilmoituspalvelu (APNS) on määritettävä tai uusittava.</span><span class="sxs-lookup"><span data-stu-id="9ce99-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="9ce99-108">Tässä [asiakirjassa](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) on ohjeet sen käyttämiseen.</span><span class="sxs-lookup"><span data-stu-id="9ce99-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="9ce99-109">**Käyttöoikeustyyppi ei kelpaa tai käyttäjänimeä ei tunnisteta:** Käyttäjälle on annettava Intune- tai EMS-lisenssi.</span><span class="sxs-lookup"><span data-stu-id="9ce99-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="9ce99-110">Tarkista nämä asiakirjat ja määritä käyttöoikeus: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) tai [Azure-portaali](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="9ce99-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="9ce99-111">Lisäresursseja ongelman ratkaisemiseen:</span><span class="sxs-lookup"><span data-stu-id="9ce99-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="9ce99-112">[Intune Troubleshooting Portalin](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) avulla voit diagnosoida ja ratkaista yleisiä rekisteröintivirheitä.</span><span class="sxs-lookup"><span data-stu-id="9ce99-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="9ce99-113">Lisätietoja on [tässä asiakirjassa.](https://docs.microsoft.com/intune/help-desk-operators)</span><span class="sxs-lookup"><span data-stu-id="9ce99-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="9ce99-114">Näissä asiakirjoissa on luettelo yleisistä virheistä, jotka estävät rekisteröitymisen ja tarkkuuden kuhunkin: [Vianmääritysopas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ja [Vianmääritysasiakirja](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="9ce99-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="9ce99-115">[Lue, miten voit rekisteröidä iOS-laitteet Microsoft Intuneen](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="9ce99-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

