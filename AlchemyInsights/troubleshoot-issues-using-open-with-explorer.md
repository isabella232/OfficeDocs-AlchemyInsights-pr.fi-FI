---
title: Avaa Resurssienhallinnassa-toiminnolla-ongelmien vian määritys
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742730"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="1faa0-102">Avaa Resurssienhallinnan ongelmien korjaaminen</span><span class="sxs-lookup"><span data-stu-id="1faa0-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="1faa0-103">Korjaa yleisiä ongelmia asiakirja kirjaston avaamisessa SharePointissa tai OneDrivessa **Avaa Resurssienhallinnassa-** komennolla:</span><span class="sxs-lookup"><span data-stu-id="1faa0-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="1faa0-104">Käytä Internet Explorer 10: tä tai Internet Explorer 11: tä.</span><span class="sxs-lookup"><span data-stu-id="1faa0-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="1faa0-105">**Avaa Explorerilla** ei ole yhteensopiva Microsoft Edgen, Google Chromen, Firefoxin ja muiden kanssa.</span><span class="sxs-lookup"><span data-stu-id="1faa0-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="1faa0-106">**Avaa Resurssienhallinnassa** ei ole käytössä kaikissa selaimissa, paitsi Internet Explorerissa.</span><span class="sxs-lookup"><span data-stu-id="1faa0-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="1faa0-107">**Avaa Resurssienhallinnassa** ei ole käytettävissä modernissa SharePoint-kirjastojen käyttö kokemessa.</span><span class="sxs-lookup"><span data-stu-id="1faa0-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="1faa0-108">Käytä sen sijaan **näkymää Resurssienhallinnassa** .</span><span class="sxs-lookup"><span data-stu-id="1faa0-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="1faa0-109">Valitse Resurssienhallinnan **Näytä asetukset** \> **-näkymä**.</span><span class="sxs-lookup"><span data-stu-id="1faa0-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="1faa0-110">View in File Explorer ei ole yhteensopiva Microsoft Edge, Google Chrome, Firefox ja muut.</span><span class="sxs-lookup"><span data-stu-id="1faa0-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="1faa0-111">**View in File Explorer** käytettävissä vain Internet Explorerissa.</span><span class="sxs-lookup"><span data-stu-id="1faa0-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="1faa0-112">Varmista, että WebClient-palvelu on käynnissä.</span><span class="sxs-lookup"><span data-stu-id="1faa0-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="1faa0-113">Kirjoita Windows Search-ruutuun Suorita, valitse Suorita Työpöytä sovellus, kirjoita Services. msc ja paina sitten ENTER-näppäintä.</span><span class="sxs-lookup"><span data-stu-id="1faa0-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="1faa0-114">Vieritä alaspäin WebClient-palveluun ja varmista, että **tila** sarakkeessa näkyy "Running".</span><span class="sxs-lookup"><span data-stu-id="1faa0-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="1faa0-115">Jos se ei ole, kaksoisnapsauta palvelua, valitse **Käynnistä**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="1faa0-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="1faa0-116">(Sinun on ehkä ensin otettava palvelu käyttöön valitsemalla **Käynnistys tyyppi** -ruudusta joko **Manuaalinen** tai **Automaattinen** .)</span><span class="sxs-lookup"><span data-stu-id="1faa0-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="1faa0-117">Kirjaston avaaminen Resurssienhallinnassa on kätevää, jos sinun on kopioitava tai siirrettävä useita tiedostoja ja kansioita kerran, mutta jos haluat työskennellä säännöllisesti kirjastossa, suosittelemme sen synkronoimista.</span><span class="sxs-lookup"><span data-stu-id="1faa0-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="1faa0-118">Jos haluat suorittaa Resurssienhallinnan ongelmien vian määrityksen, katso [Avaa Resurssienhallinnassa](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="1faa0-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="1faa0-119">Lisä tietoja synkronoinnin määrittämisestä [on artikkelissa SharePoint-tiedostojen synkronointi uuden OneDrive-synkronointi asiakkaan kanssa](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="1faa0-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="1faa0-120">Katso lisä tietoja artikkelista [kuinka käyttää avaa Exploreria-komentoa SharePoint Onlinen ongelmien vian määritykseen](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) .</span><span class="sxs-lookup"><span data-stu-id="1faa0-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

