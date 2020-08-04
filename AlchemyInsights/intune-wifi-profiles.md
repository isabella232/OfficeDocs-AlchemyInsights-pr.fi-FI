---
title: Intune Wi-Fi-profiilit
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555006"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="d076e-102">Intune Wi-Fi-profiilit</span><span class="sxs-lookup"><span data-stu-id="d076e-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="d076e-103">Wi-Fi-yhteyden onnistunut käyttöönotto MDM-asiakkaille riippuu oikein käyttöön otetusta profiilista, joka vastaa yrityksen Wi-Fi-infrastruktuurin vaatimuksia.</span><span class="sxs-lookup"><span data-stu-id="d076e-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="d076e-104">Jos haluat tarkastella tutkimiesi asiakasympäristöjen asetuksia, katso:</span><span class="sxs-lookup"><span data-stu-id="d076e-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="d076e-105">Wi-Fi-asetusten lisääminen laitteille, joissa on Android Microsoft Intunen</span><span class="sxs-lookup"><span data-stu-id="d076e-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="d076e-106">Wi-Fi-asetusten lisääminen Android Enterprise -omistautuneille ja täysin hallituille laitteille Microsoft Intunen avulla</span><span class="sxs-lookup"><span data-stu-id="d076e-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="d076e-107">Wi-Fi-asetusten lisääminen iOS- ja iPadOS-laitteille Microsoft Intutiin</span><span class="sxs-lookup"><span data-stu-id="d076e-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="d076e-108">Wi-Fi-asetusten lisääminen Windows 10:lle ja uudemmillesi laitteille Intutiin</span><span class="sxs-lookup"><span data-stu-id="d076e-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="d076e-109">Wi-Fi-asetusten tuominen Windows-laitteille Intuessa</span><span class="sxs-lookup"><span data-stu-id="d076e-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="d076e-110">**Yleisiä ongelmia**</span><span class="sxs-lookup"><span data-stu-id="d076e-110">**Common Issues**</span></span>

<span data-ttu-id="d076e-111">**Otan käyttöön Wi-Fi-profiilin, joka on riippuvainen Wi-Fi-profiilissa määritetystä käyttöönottannista varmenteesta. Määritysprofiileissa näkyy kuitenkin virheen tila.**</span><span class="sxs-lookup"><span data-stu-id="d076e-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="d076e-112">Tarkista, että laitteesi on saanut varmenteen.</span><span class="sxs-lookup"><span data-stu-id="d076e-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="d076e-113">Valitse Intunessa **Kaikki laitteet** ja valitse laite > **Laiteasetukset**.</span><span class="sxs-lookup"><span data-stu-id="d076e-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="d076e-114">Tarkista, että kaikki odotetut profiilit on lueteltu ja että ne ovat onnistuneessa tilassa.</span><span class="sxs-lookup"><span data-stu-id="d076e-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="d076e-115">Jos sinulla on Android-profiilissa välivarmenteita varmenneketjussasi, varmista, että ne on otettu käyttöön Android-laitteissa.</span><span class="sxs-lookup"><span data-stu-id="d076e-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="d076e-116">Voit tarkistaa varmenteen tilan siirtymällä **kohtaan Laitteen**  >  **määritysprofiilit**  >  **Android intermediate CA**  >  **Properties**  >  **Trusted Certificate**.</span><span class="sxs-lookup"><span data-stu-id="d076e-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="d076e-117">Jos virheet jatkuvat, tutustu toimintosarjoihin ja vianmääritysosioihin.</span><span class="sxs-lookup"><span data-stu-id="d076e-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="d076e-118">Lisätietoja on [ohjeaiheessa Scep-varmenneprofiilien vianmääritys Microsoft Intunen avulla](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="d076e-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="d076e-119">**Olen ottanut Wi-Fi-profiilin käyttöön laitteessa. Intune näyttää, että se onnistui, mutta laite ei muodosta yhteyttä Wi-Fi-verkkoon.**</span><span class="sxs-lookup"><span data-stu-id="d076e-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="d076e-120">Onnistunut tila tarkoittaa, että Intune on ottanut profiilin onnistuneesti käyttöön määritetyllä tavalla.</span><span class="sxs-lookup"><span data-stu-id="d076e-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="d076e-121">Nämä määritykset eivät kuitenkaan välttämättä vastaa verkko- ja/tai todennusvaatimuksia.</span><span class="sxs-lookup"><span data-stu-id="d076e-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="d076e-122">Lisätietoja yhteyden yrittämisestä on infrastruktuuri- ja todennuspalvelun lokeissa (Wi-Fi-tukiaseman ohjaimessa ja NPS/Radius-palvelimessa).</span><span class="sxs-lookup"><span data-stu-id="d076e-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="d076e-123">Saatat joutua työskentelemään verkkoinfrastruktuuritiimin tai kolmannen osapuolen Wi-Fi-toimittajan kanssa lokien keräämiseksi ja tarkistamiseksi.</span><span class="sxs-lookup"><span data-stu-id="d076e-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>