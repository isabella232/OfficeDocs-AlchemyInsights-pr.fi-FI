---
title: Ohjeita yövalon näyttöasetukseen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404400"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="b8b1d-102">Ohjeita yövalon näyttöasetukseen</span><span class="sxs-lookup"><span data-stu-id="b8b1d-102">Help with the night light display setting</span></span>

<span data-ttu-id="b8b1d-103">Lisätietoja yönäytön asetuksista on ohjeaiheessa Näytön [määrittäminen yöksi Windows 10:ssä.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)</span><span class="sxs-lookup"><span data-stu-id="b8b1d-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="b8b1d-104">Jos yövalon asetukset näkyvät harmaina Asetuksissa, tarkista näyttöohjain:</span><span class="sxs-lookup"><span data-stu-id="b8b1d-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="b8b1d-105">Napsauta tehtäväpalkin hakuruutua, kirjoita **Laitehallinta** ja valitse sitten **hakutuloksista** Laitehallinta.</span><span class="sxs-lookup"><span data-stu-id="b8b1d-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="b8b1d-106">Laajenna **näyttösovittimet.**</span><span class="sxs-lookup"><span data-stu-id="b8b1d-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="b8b1d-107">Yövalotoiminto ei valitettavasti ole käytettävissä, jos laitteessasi on DisplayLink-ohjain tai perusnäyttöohjain.</span><span class="sxs-lookup"><span data-stu-id="b8b1d-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="b8b1d-108">Yövalo-ominaisuus käyttää viimeaikaista grafiikkatekniikkaa, joten sinun on ehkä päivitettävä näyttöohjain:</span><span class="sxs-lookup"><span data-stu-id="b8b1d-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="b8b1d-109">Tarkista päivitykset valitsemalla Windows  >  Updaten **suojauspäivityksen**  >  **&**  >  **aloitusasetusten**  >  **päivitys.**</span><span class="sxs-lookup"><span data-stu-id="b8b1d-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="b8b1d-110">TAI</span><span class="sxs-lookup"><span data-stu-id="b8b1d-110">OR</span></span>

- <span data-ttu-id="b8b1d-111">Siirry laitteistovalmistajan tukisivustoon ja lataa ja asenna uusimmat näytönohjaimet manuaalisesti.</span><span class="sxs-lookup"><span data-stu-id="b8b1d-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="b8b1d-112">Rekisterin yövalon nollaaminen</span><span class="sxs-lookup"><span data-stu-id="b8b1d-112">Reset night light in the registry</span></span>

<span data-ttu-id="b8b1d-113">Jos näytönohjaimen päivittäminen ei toiminut, sinun on ehkä palautettava rekisterin yövalo.</span><span class="sxs-lookup"><span data-stu-id="b8b1d-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="b8b1d-114">**Varoitus:** Tätä vianmääritysvaihetta suositellaan vain kokeneille käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="b8b1d-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="b8b1d-115">Rekisterin virheellinen muokkaaminen voi aiheuttaa vakavia ongelmia.</span><span class="sxs-lookup"><span data-stu-id="b8b1d-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="b8b1d-116">Jos haluat suojauksen, varmuuskopioi rekisteri ennen sen muokkaamista, jotta voit palauttaa sen, jos ongelmia ilmenee.</span><span class="sxs-lookup"><span data-stu-id="b8b1d-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="b8b1d-117">Kirjoita hakuruutuun **regedit ja** valitse **sitten** hakutuloksista Rekisterieditori.</span><span class="sxs-lookup"><span data-stu-id="b8b1d-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="b8b1d-118">Siirry seuraavaan rekisteriavaimeen:</span><span class="sxs-lookup"><span data-stu-id="b8b1d-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="b8b1d-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="b8b1d-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="b8b1d-120">Vie ja poista seuraava aliavain:$$windows.data.bluelightred disclaimer.bluelightredstate</span><span class="sxs-lookup"><span data-stu-id="b8b1d-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="b8b1d-121">Vie ja poista seuraava aliavain:$$windows.data.bluelightred disclaimer.settings</span><span class="sxs-lookup"><span data-stu-id="b8b1d-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="b8b1d-122">Käynnistä Windows uudelleen ja tarkista, onko yövaloasetukset käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="b8b1d-122">Restart Windows and verify if the night light options are available.</span></span>


