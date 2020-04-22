---
title: Android-laitteiden rekisteröiminen Microsoft Intunen ongelmien vianmääritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759617"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="48b5b-102">Android-laitteiden rekisteröiminen Microsoft Intunen ongelmien vianmääritys</span><span class="sxs-lookup"><span data-stu-id="48b5b-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="48b5b-103">Ratkaise ongelma nyt alla olevien resurssien avulla.</span><span class="sxs-lookup"><span data-stu-id="48b5b-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="48b5b-104">Joitakin yleisiä kysymyksiä ja ratkaisuvaiheita:</span><span class="sxs-lookup"><span data-stu-id="48b5b-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="48b5b-105">**Laite, joka ei ole salattu -virhe yritysportaalissa:** Androidin uudemmat versiot, erityisesti versiosta 7.0 alkaen, edellyttävät käynnistyskoodia varmistaaksesi, että laitteesi on täysin salattu.</span><span class="sxs-lookup"><span data-stu-id="48b5b-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="48b5b-106">Yleisiä ratkaisuja ovat käynnistysnastan käyttöönotto tai laitteen salaaminen kokonaan.</span><span class="sxs-lookup"><span data-stu-id="48b5b-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="48b5b-107">Lisätietoja on [tässä asiakirjassa.](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)</span><span class="sxs-lookup"><span data-stu-id="48b5b-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="48b5b-108">**Laitteet eivät voi kirjautua sisään Intune-palvelulla tai näyttää intune-hallintakonsolissa epäterveellisinä:** Jotkin Samsung 4.4- ja Samsung 5.5 -laitteet eivät välttämättä kirjaudu palveluun.</span><span class="sxs-lookup"><span data-stu-id="48b5b-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="48b5b-109">Tähän ongelmaan on kolme mahdollista ratkaisua:</span><span class="sxs-lookup"><span data-stu-id="48b5b-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="48b5b-110">Avaa Intune Company Portal -sovellus manuaalisesti, joka käynnistää automaattisesti laitteen synkronoinnin.</span><span class="sxs-lookup"><span data-stu-id="48b5b-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="48b5b-111">Päivitä laite Android 6.0:aan tai uudempaan.</span><span class="sxs-lookup"><span data-stu-id="48b5b-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="48b5b-112">Poista Samsung Smart Manager käytöstä hallitsemasta Intune-yritysportaalia.</span><span class="sxs-lookup"><span data-stu-id="48b5b-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="48b5b-113">Tässä [asiakirjassa](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) on lisätietoja näistä kysymyksistä ja päätöslauselmista.</span><span class="sxs-lookup"><span data-stu-id="48b5b-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="48b5b-114">**Käyttäjäkäyttöoikeustyyppi Virheellinen** tai **Käyttäjänimi ei tunnisteta -virhe:** Käyttäjälle on määritettävä Intune- tai EMS-käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="48b5b-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="48b5b-115">Tarkista nämä asiakirjat ja määritä käyttöoikeus Office-hallintakeskuksen tai Azure-portaalin kautta.</span><span class="sxs-lookup"><span data-stu-id="48b5b-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="48b5b-116">Lisäresursseja ongelman ratkaisemiseen:</span><span class="sxs-lookup"><span data-stu-id="48b5b-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="48b5b-117">[Intune Troubleshooting Portalin](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) avulla voit diagnosoida ja ratkaista yleisiä rekisteröintivirheitä.</span><span class="sxs-lookup"><span data-stu-id="48b5b-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="48b5b-118">Lisätietoja on [tässä asiakirjassa.](https://docs.microsoft.com/intune/help-desk-operators)</span><span class="sxs-lookup"><span data-stu-id="48b5b-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="48b5b-119">Tässä [asiakirjassa](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) on luettelo yleisistä virheistä, jotka estävät rekisteröitymisen ja ratkaisut kuhunkin.</span><span class="sxs-lookup"><span data-stu-id="48b5b-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="48b5b-120">[Lue, miten voit rekisteröidä Android-laitteet Microsoft Intuneen](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="48b5b-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
