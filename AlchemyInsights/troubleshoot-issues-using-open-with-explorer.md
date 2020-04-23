---
title: Open with Explorerin käyttöön liittyvien ongelmien vianmääritys
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759689"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="e08ff-102">Open with Explorerin ongelmien korjaaminen</span><span class="sxs-lookup"><span data-stu-id="e08ff-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="e08ff-103">SharePointin tai OneDriven tiedostokirjaston avaamiseen liittyvien yleisten ongelmien korjaaminen **Avaa Resurssienhallinnassa** -komennolla:</span><span class="sxs-lookup"><span data-stu-id="e08ff-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="e08ff-104">Käytä Internet Explorer 10:tä tai Internet Explorer 11:tä.</span><span class="sxs-lookup"><span data-stu-id="e08ff-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="e08ff-105">**Open with Explorer** ei ole yhteensopiva Microsoft Edgen, Google Chromen, Firefoxin ja muiden kanssa.</span><span class="sxs-lookup"><span data-stu-id="e08ff-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="e08ff-106">**Avaa Resurssienhallinnassa** on poistettu käytöstä kaikissa selaimissa Internet Exploreria lukuun ottamatta.</span><span class="sxs-lookup"><span data-stu-id="e08ff-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="e08ff-107">**Avaa Resurssienhallinnan avulla** ei ole käytettävissä SharePoint-kirjastojen modernissa käyttökokemuksessa.</span><span class="sxs-lookup"><span data-stu-id="e08ff-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="e08ff-108">Käytä sen sijaan **Resurssienhallinnassa näkymää.**</span><span class="sxs-lookup"><span data-stu-id="e08ff-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="e08ff-109">Valitse **Resurssienhallinnassa Näytä asetukset** \> **.**</span><span class="sxs-lookup"><span data-stu-id="e08ff-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="e08ff-110">Resurssienhallinnan näkymä ei ole yhteensopiva Microsoft Edgen, Google Chromen, Firefoxin ja muiden kanssa.</span><span class="sxs-lookup"><span data-stu-id="e08ff-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="e08ff-111">**Näytä Resurssienhallinnassa,** joka on käytettävissä vain Internet Explorerissa.</span><span class="sxs-lookup"><span data-stu-id="e08ff-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="e08ff-112">Varmista, että WebClient-palvelu on käynnissä.</span><span class="sxs-lookup"><span data-stu-id="e08ff-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="e08ff-113">Kirjoita Windowsin hakuruutuun suorita, valitse Suorita työpöytäsovellus, kirjoita services.msc ja paina sitten Enter-näppäintä.</span><span class="sxs-lookup"><span data-stu-id="e08ff-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="e08ff-114">Vieritä alas WebClient-palveluun ja varmista, että **Tila-sarakkeessa** näkyy "Käynnissä".</span><span class="sxs-lookup"><span data-stu-id="e08ff-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="e08ff-115">Jos näin ei ole, kaksoisnapsauta palvelua, napsauta **Käynnistä -painiketta**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="e08ff-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="e08ff-116">(Sinun on ehkä ensin otettava palvelu käyttöön valitsemalla **Käynnistystapa-ruudusta** **Joko Manuaalinen** tai **Automaattinen.)**</span><span class="sxs-lookup"><span data-stu-id="e08ff-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="e08ff-117">Kirjaston avaaminen Resurssienhallinnassa on kätevää, jos haluat kopioida tai siirtää useita tiedostoja ja kansioita kerran, mutta jos haluat työskennellä säännöllisesti kirjastossa, suosittelemme sen synkronointia.</span><span class="sxs-lookup"><span data-stu-id="e08ff-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="e08ff-118">Lisätietoja Resurssienhallinnan avaamiseen liittyvien ongelmien vianmäärityksestä on [ohjeaiheessa AvaaMinen Resurssienhallinnassa](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="e08ff-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="e08ff-119">Lisätietoja synkronoinnin määrittämisestä on ohjeaiheessa [SharePoint-tiedostojen synkronoiminen uuden OneDrive-synkronointiohjelman kanssa](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="e08ff-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="e08ff-120">Lisätietoja on artikkelissa [SharePoint Onlinen ongelmien vianmääritys Avaa Resurssienhallinnassa -komennon avulla.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)</span><span class="sxs-lookup"><span data-stu-id="e08ff-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

