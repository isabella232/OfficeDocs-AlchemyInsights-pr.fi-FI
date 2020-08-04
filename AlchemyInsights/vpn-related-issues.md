---
title: VPN:ään liittyvät ongelmat
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554969"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="87389-102">VPN:ään liittyvät ongelmat</span><span class="sxs-lookup"><span data-stu-id="87389-102">VPN related issues</span></span>

<span data-ttu-id="87389-103">VPN-yhteyden onnistunut käyttöönotto MDM-asiakkaille riippuu käyttöönotetusta profiilista, joka vastaa oikein VPN-infrastruktuurin vaatimuksia.</span><span class="sxs-lookup"><span data-stu-id="87389-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="87389-104">Asianmukaiset asetukset tutkimillesi asiakasalustoille ovat seuraavissa ohjeissa:</span><span class="sxs-lookup"><span data-stu-id="87389-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="87389-105">Windows 10:n ja Windowsin hologrammilaitteen asetukset VPN-yhteyksien lisäämiseksi Intunen avulla</span><span class="sxs-lookup"><span data-stu-id="87389-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="87389-106">VPN-asetusten lisääminen iOS- ja iPadOS-laitteisiin Microsoft Intuessa</span><span class="sxs-lookup"><span data-stu-id="87389-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="87389-107">Android-laitteen asetukset VPN:n määrittämiseen Intunessa</span><span class="sxs-lookup"><span data-stu-id="87389-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="87389-108">VPN-asetusten lisääminen macOS-laitteisiin Microsoft Intunen avulla</span><span class="sxs-lookup"><span data-stu-id="87389-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="87389-109">Jos VPN-profiilisi käyttää varmennepohjaista todennusta, varmista, että VPN-profiiliin linkitetyt päävarmenteen ja asiakkaan todennusvarmenneprofiilit otetaan käyttöön onnistuneesti.</span><span class="sxs-lookup"><span data-stu-id="87389-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="87389-110">**Yleisiä ongelmia**</span><span class="sxs-lookup"><span data-stu-id="87389-110">**Common Issues**</span></span>

<span data-ttu-id="87389-111">**Otin VPN-profiilin käyttöön laitteessa. Intune näyttää onnistuneen, mutta laite ei muodosta yhteyttä VPN:ään.**</span><span class="sxs-lookup"><span data-stu-id="87389-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="87389-112">Onnistunut tila tarkoittaa, että Intune on ottanut profiilin onnistuneesti käyttöön määritetyllä tavalla.</span><span class="sxs-lookup"><span data-stu-id="87389-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="87389-113">Nämä määritykset eivät kuitenkaan välttämättä vastaa verkko- ja/tai todennusvaatimuksia.</span><span class="sxs-lookup"><span data-stu-id="87389-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="87389-114">Lisätietoja yhteyden yrittämisestä on infrastruktuuri- ja todennuspalvelun lokeissa (VPN-palvelimessa ja NPS/Radius-palvelimessa).</span><span class="sxs-lookup"><span data-stu-id="87389-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="87389-115">Sinun on ehkä työskenneltävä verkkoinfrastruktuuritiimisi tai kolmannen osapuolen VPN-toimittajan kanssa, jotta voit kerätä ja tarkastella lokeja.</span><span class="sxs-lookup"><span data-stu-id="87389-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="87389-116">**Kun määritän mukautetun VPN:n iOS:lle, sovelluskohtainen VPN-ominaisuus ei ole käytettävissä.**</span><span class="sxs-lookup"><span data-stu-id="87389-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="87389-117">Intunen iOS-laitteiden sovelluskohtainen VPN on tällä hetkellä saatavilla tietylle palveluntarjoajien ja kumppanien luettelolle, jonka on myös täytettävä varmenteen edellytykset ennen sovelluksenkohtaisen VPN:n määrittämistä.</span><span class="sxs-lookup"><span data-stu-id="87389-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="87389-118">Lisätietoja on kohdassa [Sovelluksen virtuaalisen yksityisverkon (VPN) määrittäminen iOS/iPadOS-laitteille Intuessa](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="87389-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="87389-119">Lisätietoja kaikista Intunen VPN-yhteystyypeistä on ohjeaiheessa [VPN-profiilien luominen vpn-palvelimiin yhdistämistä varten Intuessa](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="87389-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="87389-120">**iOS On-Demand VPN ei käynnisty, kun määritettyä toimialuetta käytetään**</span><span class="sxs-lookup"><span data-stu-id="87389-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="87389-121">Voit testata automaattisia VPN-asetuksia määrittämällä seuraavat arvot:</span><span class="sxs-lookup"><span data-stu-id="87389-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="87389-122">Haluan tehdä seuraavat toimet: **Arvioi jokainen yhteysyritys**</span><span class="sxs-lookup"><span data-stu-id="87389-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="87389-123">Valitse, haluatko muodostaa yhteyden: **Yhdistä tarvittaessa**</span><span class="sxs-lookup"><span data-stu-id="87389-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="87389-124">Kun käyttäjät voivat käyttää näitä toimialueita: **target** *kohdetoimialueen nimi*</span><span class="sxs-lookup"><span data-stu-id="87389-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="87389-125">Jos edellä mainittu kokoonpano ei onnistu, lisää seuraava elementti:</span><span class="sxs-lookup"><span data-stu-id="87389-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="87389-126">Kun tätä URL-osoitetta ei saada, pakota vpn: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="87389-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>