---
title: OneDrive-kaatumisten vian määritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664995"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="2f7b2-102">OneDrive-kaatumisten vian määritys</span><span class="sxs-lookup"><span data-stu-id="2f7b2-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="2f7b2-103">Jos OneDrive kaatuu toistuvasti, kokeile seuraavia vian määritys ohjeita:</span><span class="sxs-lookup"><span data-stu-id="2f7b2-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="2f7b2-104">**Varmista, että rekisteri avaimia ei ole valittu:**</span><span class="sxs-lookup"><span data-stu-id="2f7b2-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="2f7b2-105">Kun käytät rekisteri editoria, siirry kohtaan HKEY_LOCAL_MACHINE \Software\policiesmicrosoft\onedrive</span><span class="sxs-lookup"><span data-stu-id="2f7b2-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="2f7b2-106">Jos Disasemfilesyncpääsihteeristön arvo on 1, Avaa avain ja muuta arvoksi 0.</span><span class="sxs-lookup"><span data-stu-id="2f7b2-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="2f7b2-107">Käynnistä OneDrive manuaalisesti käynnistämällä</span><span class="sxs-lookup"><span data-stu-id="2f7b2-107">Manually launch OneDrive by going to Start</span></span> ![Paina Windows-näppäintä](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="2f7b2-109">, kirjoita haku ruutuun OneDrive ja valitse sitten OneDrive-Työpöytä sovellus.</span><span class="sxs-lookup"><span data-stu-id="2f7b2-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="2f7b2-110">**Palauta OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="2f7b2-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="2f7b2-111">Toteaa</span><span class="sxs-lookup"><span data-stu-id="2f7b2-111">Notes:</span></span>

- <span data-ttu-id="2f7b2-112">OneDriven palauttaminen katkaisee kaikki olemassa olevat synkronointi yhteydet (mukaan lukien henkilökohtainen OneDrive, jos se on määritetty).</span><span class="sxs-lookup"><span data-stu-id="2f7b2-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="2f7b2-113">Tiedostoja tai tietoja ei menetetä palauttamalla OneDrive tieto koneeseen.</span><span class="sxs-lookup"><span data-stu-id="2f7b2-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="2f7b2-114">**OneDriven palauttaminen:**</span><span class="sxs-lookup"><span data-stu-id="2f7b2-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="2f7b2-115">Avaa Suorita-valinta ikkuna painamalla näppäin yhdistelmää Windows-näppäintä ja R.</span><span class="sxs-lookup"><span data-stu-id="2f7b2-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="2f7b2-116">Kirjoita% localappdata% \Microsoft\OneDrive\onedrive.exe/reset ja paina OK.</span><span class="sxs-lookup"><span data-stu-id="2f7b2-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="2f7b2-117">Komento ikkuna voi näkyä lyhyesti.</span><span class="sxs-lookup"><span data-stu-id="2f7b2-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="2f7b2-118">Käynnistä OneDrive manuaalisesti käynnistämällä</span><span class="sxs-lookup"><span data-stu-id="2f7b2-118">Manually launch OneDrive by going to Start</span></span> ![Paina Windows-näppäintä](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="2f7b2-120">, kirjoita haku ruutuun OneDrive ja valitse sitten OneDrive-Työpöytä sovellus.</span><span class="sxs-lookup"><span data-stu-id="2f7b2-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="2f7b2-121">Toteaa</span><span class="sxs-lookup"><span data-stu-id="2f7b2-121">Notes:</span></span>

- <span data-ttu-id="2f7b2-122">Jos olet valinnut vain joidenkin kansioiden synkronoinnin ennen palauttamista, sinun on tehtävä se uudelleen, kun synkronointi on valmis.</span><span class="sxs-lookup"><span data-stu-id="2f7b2-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="2f7b2-123">Lue lisä tietoja artikkelista [Valitse, mitkä OneDrive-kansiot synkronoidaan tieto koneeseen](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   .</span><span class="sxs-lookup"><span data-stu-id="2f7b2-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="2f7b2-124">Sinun on suoritettava tämä henkilökohtaiseen OneDrive-ja OneDrive for Business-palveluun.</span><span class="sxs-lookup"><span data-stu-id="2f7b2-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>