---
title: Ääniongelmien vianmääritys Windows 10:ssä
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833288"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="648e9-102">Ääniongelmien vianmääritys Windows 10:ssä</span><span class="sxs-lookup"><span data-stu-id="648e9-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="648e9-103">**Äänen vianmäärityksen käynnistäminen**</span><span class="sxs-lookup"><span data-stu-id="648e9-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="648e9-104">Avaa [Vianmääritysasetukset](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="648e9-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="648e9-105">Valitse **Äänen**  >  **toistaminen Suorita vianmääritys**.</span><span class="sxs-lookup"><span data-stu-id="648e9-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="648e9-106">**Oletuslaitteen asetukset**</span><span class="sxs-lookup"><span data-stu-id="648e9-106">**Set the default device**</span></span>

<span data-ttu-id="648e9-107">Jos olet yhdistänyt äänilaitteeseen USB- tai HDMI-liitännällä, sinun on ehkä määritettävä tämä laite oletuslaitteeksi:</span><span class="sxs-lookup"><span data-stu-id="648e9-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="648e9-108">Avaa **Aloita**  >  **ääni** ja valitse sitten **tulosluettelosta** Ääni tai Muuta  järjestelmän ääniä.</span><span class="sxs-lookup"><span data-stu-id="648e9-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="648e9-109">Valitse **Toisto-välilehdessä** laite, valitse **Aseta oletus** ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="648e9-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="648e9-110">**Tarkista kaapelit, äänenvoimakkuus, kaiuttimet ja kuulokkeet**</span><span class="sxs-lookup"><span data-stu-id="648e9-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="648e9-111">Tarkista, ettei kaiuttimen ja kuulokkeiden yhteyksissä ole irtonaista kaapeleita, ja varmista, että ne on yhdistetty oikeaan liitäntään.</span><span class="sxs-lookup"><span data-stu-id="648e9-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="648e9-112">Tarkista virta- ja äänenvoimakkuustasot ja yritä kääntää kaikki äänenvoimakkuuden säätimet ylöspäin.</span><span class="sxs-lookup"><span data-stu-id="648e9-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="648e9-113">Joillakin kaiuttimillä ja sovelluksilla on omat äänenvoimakkuuden säätimet. sinun on ehkä tarkistamaan ne kaikki, jotta ne ovat oikealla tasolla.</span><span class="sxs-lookup"><span data-stu-id="648e9-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="648e9-114">Yritä muodostaa yhteys käyttämällä toista USB-porttia.</span><span class="sxs-lookup"><span data-stu-id="648e9-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="648e9-115">**Huomautus:** Muista, että kaiuttimet eivät ehkä toimi, kun kuulokkeet on kytketty.</span><span class="sxs-lookup"><span data-stu-id="648e9-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="648e9-116">**Tarkista Laitehallinta**</span><span class="sxs-lookup"><span data-stu-id="648e9-116">**Check Device Manager**</span></span>

<span data-ttu-id="648e9-117">Voit varmistaa, että ohjaimet ovat ajan tasalla:</span><span class="sxs-lookup"><span data-stu-id="648e9-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="648e9-118">Valitse **Käynnistä**, **kirjoita Laitehallinta** ja valitse **sitten** tulosluettelosta Laitehallinta.</span><span class="sxs-lookup"><span data-stu-id="648e9-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="648e9-119">Valitse **Ääni-, video- ja peliohjaimet**-kohdassa äänikortti, avaa se, valitse **Ohjain-välilehti** ja valitse **Päivitä ohjain**.</span><span class="sxs-lookup"><span data-stu-id="648e9-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="648e9-120">**Huomautus:** Jos Windows ei löydä uutta ohjainta, etsi ohjain laitteen valmistajan sivustosta ja noudata ohjeita.</span><span class="sxs-lookup"><span data-stu-id="648e9-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="648e9-121">**Asenna ohjain uudelleen**</span><span class="sxs-lookup"><span data-stu-id="648e9-121">**Reinstall the driver**</span></span>

<span data-ttu-id="648e9-122">Jos et voi päivittää laitehallinnan kautta tai etsiä uutta ohjainta valmistajan sivustosta, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="648e9-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="648e9-123">Napsauta Laitehallinnassa ääniohjainta hiiren kakkospainikkeella (tai paina sitä pitkään) ja valitse **Poista asennus**.</span><span class="sxs-lookup"><span data-stu-id="648e9-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="648e9-124">Käynnistä laite uudelleen, niin Windows yrittää asentaa ohjaimen uudelleen.</span><span class="sxs-lookup"><span data-stu-id="648e9-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="648e9-125">Jos ohjaimen uudelleenasentaminen ei toimi, kokeile Windowsin mukana toimitetaan yleistä ääniohjainta.</span><span class="sxs-lookup"><span data-stu-id="648e9-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="648e9-126">Napsauta laitehallinnassa ääniohjainta hiiren kakkospainikkeella (tai paina sitä pitkään) > Päivitä ohjainohjelmisto Selaa tietokoneeni ohjainohjelmistoa Valitsen laiteohjaimen tietokoneen luettelosta , valitse  >    >   **Teräväpiirtoäänilaite**, valitse **Seuraava** ja asenna se noudattamalla ohjeita.</span><span class="sxs-lookup"><span data-stu-id="648e9-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
