---
title: Android-laitteiden ilmoittamisongelmien vianmääritys Microsoft Intunessa
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830939"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="4e457-102">Android-laitteiden ilmoittamisongelmien vianmääritys Microsoft Intunessa</span><span class="sxs-lookup"><span data-stu-id="4e457-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="4e457-103">Ratkaise ongelma nyt alla lueteltujen resurssien avulla.</span><span class="sxs-lookup"><span data-stu-id="4e457-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="4e457-104">Joitakin yleisiä ongelmia ja ratkaisuvaiheita:</span><span class="sxs-lookup"><span data-stu-id="4e457-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="4e457-105">**Laite ei ole salattu -virhe yritysportaalissa:** Androidin uudempi versio, erityisesti v7.0-versiosta alkaen, edellyttää käynnistyksen tunnuskoodia, jotta voit varmistaa, että laitteesi on täysin salattu.</span><span class="sxs-lookup"><span data-stu-id="4e457-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="4e457-106">Yleisiä ratkaisuja ovat käynnistyksen PIN-koodin ottaminen käyttöön tai laitteen täysin salaaminen.</span><span class="sxs-lookup"><span data-stu-id="4e457-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="4e457-107">Katso [lisätietoja](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) tästä asiakirjasta.</span><span class="sxs-lookup"><span data-stu-id="4e457-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="4e457-108">Laitteet eivät pysty tarkistamaan intune-palvelua tai näy huonolla hetkellä **Intune-hallintakonsolissa:** Jotkin Samsung 4.4- ja 5.5-laitteet eivät välttämättä tarkista palvelua.</span><span class="sxs-lookup"><span data-stu-id="4e457-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="4e457-109">Tähän ongelmaan on kolme mahdollista ratkaisua:</span><span class="sxs-lookup"><span data-stu-id="4e457-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="4e457-110">Avaa Intune-yritysportaalisovellus manuaalisesti, joka aloittaa laitteen synkronoinnin automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="4e457-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="4e457-111">Päivitä laitteeseen Android 6.0 tai uudempi.</span><span class="sxs-lookup"><span data-stu-id="4e457-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="4e457-112">Poista Samsung Smart Manager käytöstä, jotta voit hallita Intune-yritysportaalia.</span><span class="sxs-lookup"><span data-stu-id="4e457-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="4e457-113">Tässä [asiakirjassa on](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) lisätietoja näistä ongelmista ja ratkaisuista.</span><span class="sxs-lookup"><span data-stu-id="4e457-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="4e457-114">**Käyttäjän käyttöoikeustyyppi Virheellinen** **tai Käyttäjänimi ei** tunnistettu -virhe: Käyttäjälle on oltava määritetty Intune- tai EMS-käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="4e457-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="4e457-115">Tarkista nämä asiakirjat ja määritä käyttöoikeus Office-hallintakeskuksen tai Azure-portaalin kautta.</span><span class="sxs-lookup"><span data-stu-id="4e457-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="4e457-116">Lisäresursseja ongelman ratkaisemiseksi:</span><span class="sxs-lookup"><span data-stu-id="4e457-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="4e457-117">[Intunen vianmääritysportaalin avulla voit](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) tehdä vianmäärityksen ja ratkaista yleisiä rekisteröintivirheitä.</span><span class="sxs-lookup"><span data-stu-id="4e457-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="4e457-118">Katso [lisätietoja](https://docs.microsoft.com/intune/help-desk-operators) tästä asiakirjasta.</span><span class="sxs-lookup"><span data-stu-id="4e457-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="4e457-119">Tarkista [tästä asiakirjasta](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) luettelo yleisistä virheistä, jotka estävät jokaisen rekisteröinnin ja ratkaisut.</span><span class="sxs-lookup"><span data-stu-id="4e457-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="4e457-120">[Opi rekisteröimaan Android-laitteet Microsoft Intunessa.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="4e457-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
