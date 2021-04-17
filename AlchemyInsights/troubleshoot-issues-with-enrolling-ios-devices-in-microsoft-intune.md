---
title: iOS-laitteiden rekisteröintiongelmien vianmääritys Microsoft Intunessa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823460"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="fd274-102">iOS-laitteiden rekisteröintiongelmien vianmääritys Microsoft Intunessa</span><span class="sxs-lookup"><span data-stu-id="fd274-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="fd274-103">Ratkaise ongelma nyt alla lueteltujen resurssien avulla.</span><span class="sxs-lookup"><span data-stu-id="fd274-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="fd274-104">Yleisiä virhesanomia ja ratkaisuvaiheita:</span><span class="sxs-lookup"><span data-stu-id="fd274-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="fd274-105">**Laitteen kapetin saavutettu** Käyttäjällä on laiterajoitusta suurempia laitteita.</span><span class="sxs-lookup"><span data-stu-id="fd274-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="fd274-106">Tarkista nämä [asiakirjat, jos haluat poistaa laitteen](https://docs.microsoft.com/intune/devices-wipe) tai muuttaa laitteen [rajoitusta.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="fd274-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="fd274-107">**Tätä palvelua ei tueta. Ei rekisteröintikäytäntöä:** Apple Push Notification Service (APNS) on määritettävä tai uusittava.</span><span class="sxs-lookup"><span data-stu-id="fd274-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="fd274-108">Katso [ohjeet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) tästä asiakirjasta.</span><span class="sxs-lookup"><span data-stu-id="fd274-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="fd274-109">**Käyttäjäkäyttöoikeustyyppi Virheellinen tai käyttäjänimi ei tunnistettu:** Käyttäjälle on oltava määritetty Intune- tai EMS-käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="fd274-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="fd274-110">Tarkista nämä asiakirjat ja määritä käyttöoikeus [Office-hallintakeskuksen tai](https://docs.microsoft.com/intune/licenses-assign) [Azure-portaalin kautta.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="fd274-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="fd274-111">Lisäresursseja ongelman ratkaisemiseksi:</span><span class="sxs-lookup"><span data-stu-id="fd274-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="fd274-112">[Intunen vianmääritysportaalin avulla voit](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) tehdä vianmäärityksen ja ratkaista yleisiä rekisteröintivirheitä.</span><span class="sxs-lookup"><span data-stu-id="fd274-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="fd274-113">Katso [lisätietoja](https://docs.microsoft.com/intune/help-desk-operators) tästä asiakirjasta.</span><span class="sxs-lookup"><span data-stu-id="fd274-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="fd274-114">Tarkistamalla nämä asiakirjat saat luettelon yleisistä virheistä, jotka estävät kunkin tiedoston rekisteröinnin ja ratkaisut: [Vianmääritysopas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ja [Tiedoston vianmääritys.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="fd274-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="fd274-115">[Lue, miten voit rekisteröidä iOS-laitteet Microsoft Intunessa.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="fd274-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

