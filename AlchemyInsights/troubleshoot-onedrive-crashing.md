---
title: OneDriven kaatumisen vianmääritys
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826196"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="1f503-102">OneDriven kaatumisen vianmääritys</span><span class="sxs-lookup"><span data-stu-id="1f503-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="1f503-103">Jos OneDrive kaatuu toistuvasti, kokeile seuraavia vianmääritysohjeita:</span><span class="sxs-lookup"><span data-stu-id="1f503-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="1f503-104">**Varmista, että rekisteriavaimia ei ole määritetty:**</span><span class="sxs-lookup"><span data-stu-id="1f503-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="1f503-105">Siirry rekisterieditorin avulla HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="1f503-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="1f503-106">Jos DisableFileSyncNGSC on käytössä ja sen arvona on 1, avaa avain ja muuta arvoksi 0.</span><span class="sxs-lookup"><span data-stu-id="1f503-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="1f503-107">OneDriven käynnistäminen manuaalisesti aloitusnäyttöön</span><span class="sxs-lookup"><span data-stu-id="1f503-107">Manually launch OneDrive by going to Start</span></span> ![Paina Windows-näppäintä](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="1f503-109">, kirjoita OneDrive hakuruutuun ja napsauta sitten OneDrive-työpöytäsovellusta.</span><span class="sxs-lookup"><span data-stu-id="1f503-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="1f503-110">**OneDriven palauttaminen:**</span><span class="sxs-lookup"><span data-stu-id="1f503-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="1f503-111">Huomautukset:</span><span class="sxs-lookup"><span data-stu-id="1f503-111">Notes:</span></span>

- <span data-ttu-id="1f503-112">OneDriven palauttaminen katkaisee kaikki olemassa olevat synkronointiyhteydet (mukaan lukien henkilökohtainen OneDrive, jos se on määritetty).</span><span class="sxs-lookup"><span data-stu-id="1f503-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="1f503-113">Tiedostoja tai tietoja ei menetetä palauttamalla OneDrive tietokoneessa.</span><span class="sxs-lookup"><span data-stu-id="1f503-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="1f503-114">**OneDriven palauttaminen:**</span><span class="sxs-lookup"><span data-stu-id="1f503-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="1f503-115">Avaa Suorita-valintaikkuna painamalla Windows-näppäintä ja R-näppäintä.</span><span class="sxs-lookup"><span data-stu-id="1f503-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="1f503-116">Kirjoita %localappdata%\Microsoft\OneDrive\onedrive.exe /reset ja paina OK.</span><span class="sxs-lookup"><span data-stu-id="1f503-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="1f503-117">Komentoikkuna saattaa tulla näkyviin hetkeksi.</span><span class="sxs-lookup"><span data-stu-id="1f503-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="1f503-118">OneDriven käynnistäminen manuaalisesti aloitusnäyttöön</span><span class="sxs-lookup"><span data-stu-id="1f503-118">Manually launch OneDrive by going to Start</span></span> ![Paina Windows-näppäintä](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="1f503-120">, kirjoita OneDrive hakuruutuun ja napsauta sitten OneDrive-työpöytäsovellusta.</span><span class="sxs-lookup"><span data-stu-id="1f503-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="1f503-121">Huomautukset:</span><span class="sxs-lookup"><span data-stu-id="1f503-121">Notes:</span></span>

- <span data-ttu-id="1f503-122">Jos valitsit vain joidenkin kansioiden synkronoinnin ennen palautusta, sinun on tehtävä se uudelleen, kun synkronointi on valmis.</span><span class="sxs-lookup"><span data-stu-id="1f503-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="1f503-123">Lisätietoja [on kohdassa Valitse, mitkä OneDrive-kansiot](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   synkronoidaan tietokoneeseen.</span><span class="sxs-lookup"><span data-stu-id="1f503-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="1f503-124">Tämä on tehtävä henkilökohtaisessa OneDrivessa ja OneDrive for Businessissa.</span><span class="sxs-lookup"><span data-stu-id="1f503-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>