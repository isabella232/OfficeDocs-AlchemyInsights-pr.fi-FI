---
title: Windows 10:n ääniongelmien vianmääritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: f51fd233db5ae068e719f1cf3bc94a0dac82444f
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265013"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="13148-102">Ääniongelmien vianmääritys Windows 10:ssä</span><span class="sxs-lookup"><span data-stu-id="13148-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="13148-103">**Äänen vianmäärityksen suorittaminen**</span><span class="sxs-lookup"><span data-stu-id="13148-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="13148-104">Avaa [Vianmääritysasetukset](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="13148-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="13148-105">Valitse **Äänen** > **toistaminen Suorita vianmääritys**.</span><span class="sxs-lookup"><span data-stu-id="13148-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="13148-106">**Oletuslaitteen määrittäminen**</span><span class="sxs-lookup"><span data-stu-id="13148-106">**Set the default device**</span></span>

<span data-ttu-id="13148-107">Jos muodostat yhteyden äänilaitteeseen USB- tai HDMI-liitännän avulla, sinun on ehkä asetettava kyseinen laite oletuslaitteeksi:</span><span class="sxs-lookup"><span data-stu-id="13148-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="13148-108">Avaa **Aloita** > **ääni**ja valitse sitten tulosluettelosta **Ääni** tai Muuta **järjestelmän ääniä.**</span><span class="sxs-lookup"><span data-stu-id="13148-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="13148-109">Valitse **Toisto-välilehdessä** laite, valitse **Aseta oletukseksi**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="13148-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="13148-110">**Kaapelien, äänenvoimakkuuden, kaiuttimien ja kuulokkeiden tarkistaminen**</span><span class="sxs-lookup"><span data-stu-id="13148-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="13148-111">Tarkista, ettei kaiutin- ja kuulokeliitännöissä ole irrallisia kaapeleita, ja varmista, että ne on liitetty oikeaan liitäntään.</span><span class="sxs-lookup"><span data-stu-id="13148-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="13148-112">Tarkista teho- ja äänenvoimakkuustasot ja yritä kääntää kaikki äänenvoimakkuuden säätimet ylöspäin.</span><span class="sxs-lookup"><span data-stu-id="13148-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="13148-113">Joillakin kaiuttimilla ja sovelluksilla on omat äänenvoimakkuuden säätimet; sinun on ehkä tarkistettava ne kaikki varmistaaksesi, että ne ovat oikealla tasolla.</span><span class="sxs-lookup"><span data-stu-id="13148-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="13148-114">Yritä muodostaa yhteys toisella USB-portilla.</span><span class="sxs-lookup"><span data-stu-id="13148-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="13148-115">**Huomautus**: Muista, että kaiuttimet eivät välttämättä toimi, kun kuulokkeet on kytketty.</span><span class="sxs-lookup"><span data-stu-id="13148-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="13148-116">**Tarkista Laitehallinta**</span><span class="sxs-lookup"><span data-stu-id="13148-116">**Check Device Manager**</span></span>

<span data-ttu-id="13148-117">Voit varmistaa, että ohjaimet ovat ajan tasalla:</span><span class="sxs-lookup"><span data-stu-id="13148-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="13148-118">Valitse **Käynnistä**, kirjoita **Laitehallinta**ja valitse sitten **laitehallinta** tulosluettelosta.</span><span class="sxs-lookup"><span data-stu-id="13148-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="13148-119">Valitse **Ääni-, video- ja peliohjaimet**-kohdassa äänikortti, avaa se, valitse **Ohjain-välilehti** ja valitse **Päivitä ohjain**.</span><span class="sxs-lookup"><span data-stu-id="13148-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="13148-120">**Huomautus:** Jos Windows ei löydä uutta ohjainta, etsi sellainen laitteen valmistajan sivustosta ja noudata niiden ohjeita.</span><span class="sxs-lookup"><span data-stu-id="13148-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="13148-121">**Asenna ohjain uudelleen**</span><span class="sxs-lookup"><span data-stu-id="13148-121">**Reinstall the driver**</span></span>

<span data-ttu-id="13148-122">Jos et pysty päivittämään Laitehallinnan kautta tai löytämään uuden ohjaimen valmistajan sivustosta, kokeile seuraavia toimia:</span><span class="sxs-lookup"><span data-stu-id="13148-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="13148-123">Napsauta Laitehallinnassa ääniohjainta hiiren kakkospainikkeella (tai pidä sitä painettuna) ja valitse **Poista asennus**.</span><span class="sxs-lookup"><span data-stu-id="13148-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="13148-124">Käynnistä laite uudelleen, niin Windows yrittää asentaa ohjaimen uudelleen.</span><span class="sxs-lookup"><span data-stu-id="13148-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="13148-125">Jos ohjaimen uudelleenasentaminen ei toimi, kokeile Windowsin mukana toimitetun yleisen ääniohjaimen käyttämistä.</span><span class="sxs-lookup"><span data-stu-id="13148-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="13148-126">Napsauta Laitehallinnassa hiiren kakkospainikkeella (tai pidä painettuna) ääniohjainta > **Update-ohjainohjelmisto** > **Selaa tietokonetta ohjainohjelmistoksi** > Haluan valita tietokoneen**laiteohjaimien luettelosta**, valitse High Definition Audio **Device**, valitse **Seuraava**ja asenna se noudattamalla ohjeita.</span><span class="sxs-lookup"><span data-stu-id="13148-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
