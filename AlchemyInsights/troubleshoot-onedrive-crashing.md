---
title: OneDriven kaatumisiin liittyviä ongelmia
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/15/2020
ms.locfileid: "44748918"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="f17b0-102">OneDriven kaatumisiin liittyviä ongelmia</span><span class="sxs-lookup"><span data-stu-id="f17b0-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="f17b0-103">Jos OneDrive kaatuu toistuvasti, kokeile seuraavia vianmääritysohjeita:</span><span class="sxs-lookup"><span data-stu-id="f17b0-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="f17b0-104">**Varmista, että rekisteriavaimia ei ole määritetty:**</span><span class="sxs-lookup"><span data-stu-id="f17b0-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="f17b0-105">Siirry Rekisterieditorin avulla kohtaan HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="f17b0-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="f17b0-106">Jos DisableFileSyncNGSC on olemassa ja sen arvo on 1, avaa avain ja muuta arvoksi 0.</span><span class="sxs-lookup"><span data-stu-id="f17b0-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="f17b0-107">Käynnistä OneDrive manuaalisesti käynnistämällä aloitus</span><span class="sxs-lookup"><span data-stu-id="f17b0-107">Manually launch OneDrive by going to Start</span></span> ![Paina Windows-näppäintä](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="f17b0-109">, kirjoita hakuruutuun OneDrive ja napsauta sitten OneDrive-työpöytäsovellusta.</span><span class="sxs-lookup"><span data-stu-id="f17b0-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="f17b0-110">**Nollaa OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="f17b0-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="f17b0-111">Muistiinpanoja:</span><span class="sxs-lookup"><span data-stu-id="f17b0-111">Notes:</span></span>

- <span data-ttu-id="f17b0-112">OneDriven nollaaminen katkaisee kaikki nykyiset synkronointiyhteytesi (mukaan lukien henkilökohtaisen OneDriven, jos se on määritetty).</span><span class="sxs-lookup"><span data-stu-id="f17b0-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="f17b0-113">Et menetä tiedostoja tai tietoja palauttamalla OneDriven tietokoneeseen.</span><span class="sxs-lookup"><span data-stu-id="f17b0-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="f17b0-114">**OneDriven nollaaminen:**</span><span class="sxs-lookup"><span data-stu-id="f17b0-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="f17b0-115">Avaa Suorita-valintaikkuna painamalla Windows-näppäintä ja R-näppäintä.</span><span class="sxs-lookup"><span data-stu-id="f17b0-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="f17b0-116">Kirjoita %localappdata%\Microsoft\OneDrive\onedrive.exe /reset ja paina OK-painiketta.</span><span class="sxs-lookup"><span data-stu-id="f17b0-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="f17b0-117">Komentoikkuna saattaa näkyä lyhyesti.</span><span class="sxs-lookup"><span data-stu-id="f17b0-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="f17b0-118">Käynnistä OneDrive manuaalisesti käynnistämällä aloitus</span><span class="sxs-lookup"><span data-stu-id="f17b0-118">Manually launch OneDrive by going to Start</span></span> ![Paina Windows-näppäintä](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="f17b0-120">, kirjoita hakuruutuun OneDrive ja napsauta sitten OneDrive-työpöytäsovellusta.</span><span class="sxs-lookup"><span data-stu-id="f17b0-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="f17b0-121">Muistiinpanoja:</span><span class="sxs-lookup"><span data-stu-id="f17b0-121">Notes:</span></span>

- <span data-ttu-id="f17b0-122">Jos olet valinnut vain joidenkin kansioiden synkronoinnin ennen nollausta, sinun on tehtävä se uudelleen, kun synkronointi on valmis.</span><span class="sxs-lookup"><span data-stu-id="f17b0-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="f17b0-123">Lisätietoja on kohdassa [Tietokoneeseen synkronoitavien OneDrive-kansioiden](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   valitseminen.</span><span class="sxs-lookup"><span data-stu-id="f17b0-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="f17b0-124">Sinun on suoritettava tämä henkilökohtaiseen OneDriveen ja OneDrive for Businessiin.</span><span class="sxs-lookup"><span data-stu-id="f17b0-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>