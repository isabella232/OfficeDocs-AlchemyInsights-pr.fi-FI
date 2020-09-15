---
title: Android-laitteiden rekisteröimisen ongelmien vian määritys Microsoft Intunella
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
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689951"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="e0538-102">Android-laitteiden rekisteröimisen ongelmien vian määritys Microsoft Intunella</span><span class="sxs-lookup"><span data-stu-id="e0538-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="e0538-103">Ratkaise ongelma nyt alla lueteltujen resurssien avulla.</span><span class="sxs-lookup"><span data-stu-id="e0538-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="e0538-104">Yleisiä ongelmia ja ratkaisu vaiheita:</span><span class="sxs-lookup"><span data-stu-id="e0538-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="e0538-105">**Laite ei ole salattu virhe yritys portaalissa:** Androidin uudemmat versiot, erityisesti v 7.0:n versiosta alkaen, vaativat käynnistys tunnus koodin, jolla varmistetaan, että laitteesi on täysin salattu.</span><span class="sxs-lookup"><span data-stu-id="e0538-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="e0538-106">Yleisiä ratkaisuja on ottaa käyttöön käynnistys PIN-koodi tai täysin salata laite.</span><span class="sxs-lookup"><span data-stu-id="e0538-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="e0538-107">Katso lisä tietoja [tästä asia kirjasta](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) .</span><span class="sxs-lookup"><span data-stu-id="e0538-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="e0538-108">**Laitteet eivät ole sisäänkuittausta Intune-palvelussa tai ne näkyvät Epäterveinä Intune-hallinta konsolissa:** Jotkin Samsung 4,4-ja 5,5-laitteet eivät välttämättä Tarkista palvelua.</span><span class="sxs-lookup"><span data-stu-id="e0538-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="e0538-109">Tähän ongelmaan on kolme mahdollista ratkaisua:</span><span class="sxs-lookup"><span data-stu-id="e0538-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="e0538-110">Avaa Intune Company Portal-sovellus manuaalisesti, joka käynnistää automaattisesti laitteen synkronoinnin.</span><span class="sxs-lookup"><span data-stu-id="e0538-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="e0538-111">Päivitä laite Android 6,0 tai uudempaan versioon.</span><span class="sxs-lookup"><span data-stu-id="e0538-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="e0538-112">Poista Samsung Smart-hallinta käytöstä Intune-yritys portaalin Hallin nasta.</span><span class="sxs-lookup"><span data-stu-id="e0538-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="e0538-113">Katso lisä tietoja näistä ongelmista ja ratkaisuista lukemalla [Tämä asia kirja](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) .</span><span class="sxs-lookup"><span data-stu-id="e0538-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="e0538-114">**Käyttö oikeuden tyyppi ei kelpaa** tai **käyttäjä nimi ei tunnista virhettä:** käyttäjälle on määritetään INTUNE-tai EMS-käyttö oikeus.</span><span class="sxs-lookup"><span data-stu-id="e0538-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="e0538-115">Voit määrittää käyttö oikeuden seuraavien tiedostojen avulla: Office-hallinta keskus tai Azure-portaali.</span><span class="sxs-lookup"><span data-stu-id="e0538-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="e0538-116">Lisä resursseja ongelman ratkaisemiseen:</span><span class="sxs-lookup"><span data-stu-id="e0538-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="e0538-117">Käytä [Intune-vian määritys portaalia](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) yleisten rekisteröinti virheiden diagnosointiin ja ratkaisemiseen.</span><span class="sxs-lookup"><span data-stu-id="e0538-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="e0538-118">Katso lisä tietoja [tästä asia kirjasta](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="e0538-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="e0538-119">Tarkista [Tämä asia kirja](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) , jossa on luettelo yleisistä virheistä, jotka estävät rekisteröinnin ja päätös lauselmien kunkin.</span><span class="sxs-lookup"><span data-stu-id="e0538-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="e0538-120">[Opi rekisteröimään Android-laitteet Microsoft Intunella](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="e0538-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
