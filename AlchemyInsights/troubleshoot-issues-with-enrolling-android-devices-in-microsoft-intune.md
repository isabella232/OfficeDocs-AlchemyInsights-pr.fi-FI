---
title: Android-laitteiden rekisteröintiongelmien vianmääritys Microsoft Intunessa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708995"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="41838-102">Android-laitteiden rekisteröintiongelmien vianmääritys Microsoft Intunessa</span><span class="sxs-lookup"><span data-stu-id="41838-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="41838-103">Ratkaise ongelmasi nyt alla lueteltujen resurssien avulla.</span><span class="sxs-lookup"><span data-stu-id="41838-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="41838-104">Joitakin yleisiä ongelmia ja ratkaisuvaiheita:</span><span class="sxs-lookup"><span data-stu-id="41838-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="41838-105">**Laite ei ole salattu -virhe yritysportaalissa:** Androidin uudempien versioiden, erityisesti v7.0-version, on oltava käynnistyksen tunnuskoodi, jotta varmistat, että laitteesi on täysin salattu.</span><span class="sxs-lookup"><span data-stu-id="41838-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="41838-106">Yleisiä ratkaisuja ovat käynnistystallenuksen ottaminen käyttöön tai laitteen täysin salaaminen.</span><span class="sxs-lookup"><span data-stu-id="41838-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="41838-107">Katso [lisätietoja tästä](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) asiakirjasta.</span><span class="sxs-lookup"><span data-stu-id="41838-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="41838-108">**Laitteet eivät pysty sisään Intune-palvelussa tai näkyvät epäterveellisenä Intune-hallintakonsolissa:** Jotkin Samsung 4.4- ja 5.5-laitteet eivät välttämättä tarkista palvelua.</span><span class="sxs-lookup"><span data-stu-id="41838-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="41838-109">Tähän ongelmaan on kolme mahdollista ratkaisua:</span><span class="sxs-lookup"><span data-stu-id="41838-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="41838-110">Avaa Manuaalisesti Intune-yritysportaalisovellus, joka aloittaa laitteen synkronoinnin automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="41838-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="41838-111">Päivitä laite Android 6.0-versioon tai sitä uudempiin versioihin.</span><span class="sxs-lookup"><span data-stu-id="41838-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="41838-112">Poista Samsung Smart Manager käytöstä hallitsemalla Intune-yritysportaalia.</span><span class="sxs-lookup"><span data-stu-id="41838-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="41838-113">Tässä [asiakirjassa on](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) lisätietoja näistä ongelmista ja ratkaisuista.</span><span class="sxs-lookup"><span data-stu-id="41838-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="41838-114">**Käyttäjäkäyttöoikeustyyppi** **virheellinen tai käyttäjänimiä** ei tunnisteta -virhe: Käyttäjälle on oltava määritetty Intune- tai EMS-käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="41838-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="41838-115">Tarkista nämä tiedostot ja määritä käyttöoikeus Office-hallintakeskuksen tai Azure-portaalin kautta.</span><span class="sxs-lookup"><span data-stu-id="41838-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="41838-116">Lisäresursseja ongelman ratkaisemiseen:</span><span class="sxs-lookup"><span data-stu-id="41838-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="41838-117">[Intunen vianmääritysportaalin avulla](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) voit diagnosoida ja ratkaista yleisiä rekisteröintivirheitä.</span><span class="sxs-lookup"><span data-stu-id="41838-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="41838-118">Katso [lisätietoja tästä](https://docs.microsoft.com/intune/help-desk-operators) asiakirjasta.</span><span class="sxs-lookup"><span data-stu-id="41838-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="41838-119">Tässä [asiakirjassa on](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) luettelo yleisistä virheistä, jotka estävät kunkin rekisteröinnin ja ratkaisut.</span><span class="sxs-lookup"><span data-stu-id="41838-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="41838-120">[Opi rekisteröimaan Android-laitteet Microsoft Intunessa.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="41838-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
