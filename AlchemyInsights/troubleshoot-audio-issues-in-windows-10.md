---
title: 'Ääni ongelmien vian määritys Windows 10: ssä'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750304"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="1a949-102">Ääni ongelmien vian määritys Windows 10: ssä</span><span class="sxs-lookup"><span data-stu-id="1a949-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="1a949-103">**Äänen vian määrityksen suorittaminen**</span><span class="sxs-lookup"><span data-stu-id="1a949-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="1a949-104">Avaa [vian määritys-asetukset](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="1a949-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="1a949-105">Valitse **äänen toistaminen**  >  **Suorita vian määritys**.</span><span class="sxs-lookup"><span data-stu-id="1a949-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="1a949-106">**Oletus laitteen asettaminen**</span><span class="sxs-lookup"><span data-stu-id="1a949-106">**Set the default device**</span></span>

<span data-ttu-id="1a949-107">Jos muodostat yhteyden ääni laitteeseen USB-tai HDMI-liitännällä, sinun on ehkä määritettävä tämä laite oletukseksi:</span><span class="sxs-lookup"><span data-stu-id="1a949-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="1a949-108">Avaa **Aloita**  >  **ääni**ja valitse sitten tulosten luettelosta **ääni** tai **muuta järjestelmän ääniä** .</span><span class="sxs-lookup"><span data-stu-id="1a949-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="1a949-109">Valitse **toisto** -väli lehdessä laite, valitse **Aseta oletukseksi**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="1a949-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="1a949-110">**Kaapelien, äänen, kaiuttimien ja kuulokkeiden tarkistaminen**</span><span class="sxs-lookup"><span data-stu-id="1a949-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="1a949-111">Tarkista kaiutin-ja kuuloke liitännät irrallisia kaapeleita varten ja varmista, että ne on liitetty oikeaan liitäntään.</span><span class="sxs-lookup"><span data-stu-id="1a949-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="1a949-112">Tarkista virta-ja ääni tasot ja yritä kääntää kaikki ääni säädöt ylöspäin.</span><span class="sxs-lookup"><span data-stu-id="1a949-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="1a949-113">Joillakin kaiuttimilla ja sovelluksilla on omat ääni asetukset. sinun on ehkä tarkistettava ne kaikki varmistaaksesi, että ne ovat oikealla tasolla.</span><span class="sxs-lookup"><span data-stu-id="1a949-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="1a949-114">Yritä muodostaa yhteys käyttämällä toista USB-porttia.</span><span class="sxs-lookup"><span data-stu-id="1a949-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="1a949-115">**Huomautus**: muista, että kaiuttimet eivät välttämättä toimi, kun kuulokkeet on kytketty.</span><span class="sxs-lookup"><span data-stu-id="1a949-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="1a949-116">**Tarkista laite hallinnasta**</span><span class="sxs-lookup"><span data-stu-id="1a949-116">**Check Device Manager**</span></span>

<span data-ttu-id="1a949-117">Varmista, että ohjaimet ovat ajan tasalla:</span><span class="sxs-lookup"><span data-stu-id="1a949-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="1a949-118">Valitse **Käynnistä**, kirjoita **laite hallintaan**ja valitse sitten Haku tulosten luettelosta **laite hallintaan** .</span><span class="sxs-lookup"><span data-stu-id="1a949-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="1a949-119">Valitse **ääni-, video-ja peli ohjaimet**-kohdassa ääni korttisi, avaa se, valitse **ohjain** -väli lehti ja valitse sitten **Päivitä ohjain**.</span><span class="sxs-lookup"><span data-stu-id="1a949-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="1a949-120">**Huomautus**: Jos Windows ei löydä uutta ohjainta, Etsi jokin laite valmistajan sivustosta ja noudata niiden ohjeita.</span><span class="sxs-lookup"><span data-stu-id="1a949-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="1a949-121">**Ohjaimen asentaminen uudelleen**</span><span class="sxs-lookup"><span data-stu-id="1a949-121">**Reinstall the driver**</span></span>

<span data-ttu-id="1a949-122">Jos et voi päivittää laite hallintaa tai etsiä uutta ohjainta valmistajan verkkosivustosta, kokeile seuraavia ohjeita:</span><span class="sxs-lookup"><span data-stu-id="1a949-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="1a949-123">Napsauta laite hallinnasta hiiren kakkos painikkeella (tai paina pitkään) ääni ohjainta ja valitse **Poista asennus**.</span><span class="sxs-lookup"><span data-stu-id="1a949-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="1a949-124">Käynnistä laite uudelleen ja Windows yrittää asentaa ohjaimen uudelleen.</span><span class="sxs-lookup"><span data-stu-id="1a949-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="1a949-125">Jos ohjaimen uudelleenasennus ei onnistu, kokeile käyttää Windowsin mukana tulevaa yleistä ääni ohjainta.</span><span class="sxs-lookup"><span data-stu-id="1a949-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="1a949-126">Napsauta laite hallinnasta hiiren kakkos painikkeella (tai paina pitkään) ääni ohjainta > **Päivitä ohjain ohjelmisto**  >  **Etsi ohjain ohjelmistoa tieto**koneesta valitsemalla  >  **laite ohjainten luettelosta oma tieto kone**, valitse **teräväpiirto-ääni laite**, valitse **Seuraava**ja noudata asennus ohjeita.</span><span class="sxs-lookup"><span data-stu-id="1a949-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
