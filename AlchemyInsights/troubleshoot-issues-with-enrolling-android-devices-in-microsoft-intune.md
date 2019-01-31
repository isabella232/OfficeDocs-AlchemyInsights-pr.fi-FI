---
title: Rekisteröiminen Microsoft Intune Android-laitteiden ongelmien vianmääritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 6b26b2d77bceb063090986ff4e20bc4a56bb1242
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655880"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="d1639-102">Rekisteröiminen Microsoft Intune Android-laitteiden ongelmien vianmääritys</span><span class="sxs-lookup"><span data-stu-id="d1639-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="d1639-103">Tarkista ongelman nyt alla luetellut resurssit.</span><span class="sxs-lookup"><span data-stu-id="d1639-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="d1639-104">Joitakin yleisiä ongelmia ja tarkkuutta vaiheet:</span><span class="sxs-lookup"><span data-stu-id="d1639-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="d1639-p101">**Laite ole salattu virhe yrityksen portaali:** Android, alkaen v7.0, erityisesti uudemmat versiot vaativat käynnistyksen PIN-koodi, varmista, että laite on täysin salattu. Yhteisiä ratkaisuja, jotka käyttöön käynnistyksen PIN-tunnuksen tai laitteen täysin salaa. Lisätietoja [tämän asiakirjan](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) tarkasteleminen.</span><span class="sxs-lookup"><span data-stu-id="d1639-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="d1639-p102">**Laitteet eivät Intune palvelu tulee tarkistaa tai näyttää Intune hallintakonsolissa ”Unhealthy”:** Jotkut Samsung 4.4 ja 5.5 laitteet ei välttämättä tarkista palveluun. 3 mahdollisia ratkaisuja tähän ongelmaan on:</span><span class="sxs-lookup"><span data-stu-id="d1639-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="d1639-110">Avaa app Intune yrityksen portaali, jossa laitteen synkronointi automaattisesti aloittaa manuaalisesti.</span><span class="sxs-lookup"><span data-stu-id="d1639-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="d1639-111">Päivitä laitteen Android 6.0 tai uudempi versio.</span><span class="sxs-lookup"><span data-stu-id="d1639-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="d1639-p103">Samsung Smart hallinnan käytöstä hallitsemasta Intune yrityksen portaaliin. Lue [Tämä asiakirja](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) on lisätietoja näistä ongelmista ja ratkaisuja.</span><span class="sxs-lookup"><span data-stu-id="d1639-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="d1639-p104">**Käyttäjän käyttöoikeuden tyyppi ei kelpaa** tai **Virhe käyttäjän nimeä ei tunnistettu:** käyttäjä on varattava Intune tai EMS-käyttöoikeus. Tarkasteltava näitä asiakirjoja käyttöoikeuden kautta: Office Admin Centerissä tai Azure portal.</span><span class="sxs-lookup"><span data-stu-id="d1639-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="d1639-116">Lisätietoja ja resursseja auttaa ratkaisemaan ongelmaasi:</span><span class="sxs-lookup"><span data-stu-id="d1639-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="d1639-p105">[Intune vianmääritys-portaalin](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) avulla voit diagnosoida ja ratkaista yhteisen rekisteröinti virheitä. Lisätietoja [tämän asiakirjan](https://docs.microsoft.com/intune/help-desk-operators) tarkasteleminen.</span><span class="sxs-lookup"><span data-stu-id="d1639-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="d1639-119">Yleisiä virheitä, jotka estävät rekisteröinti ja ratkaisuja jokaiseen luettelo [tämän asiakirjan](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) tarkasteleminen.</span><span class="sxs-lookup"><span data-stu-id="d1639-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="d1639-120">[Rekisteröi Microsoft Intune Android-laitteiden tietoja](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="d1639-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
    

