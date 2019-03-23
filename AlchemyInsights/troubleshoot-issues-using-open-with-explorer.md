---
title: Käyttämällä Avaa Explorerin ongelmien vianmääritys
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
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/22/2019
ms.locfileid: "30759291"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="0740e-102">Avaa Explorer liittyvien ongelmien korjaaminen</span><span class="sxs-lookup"><span data-stu-id="0740e-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="0740e-103">Yleisten ongelmien avaamalla asiakirjakirjaston SharePoint- tai OneDrive **Avaa Explorerissa** -komennolla:</span><span class="sxs-lookup"><span data-stu-id="0740e-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="0740e-104">Käytä Internet Explorer 10 tai Internet Explorerin 11.</span><span class="sxs-lookup"><span data-stu-id="0740e-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="0740e-105">**Avaa Explorerissa** ei ole yhteensopiva Microsoft Edge, Google Chrome, Firefox ja muut.</span><span class="sxs-lookup"><span data-stu-id="0740e-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="0740e-106">**Avaa Explorerissa** ei ole käytettävissä kaikissa selaimissa kuin Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="0740e-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="0740e-107">**Avaa Explorerissa** ei ole käytettävissä SharePoint-kirjastoihin, Moderni kokemus.</span><span class="sxs-lookup"><span data-stu-id="0740e-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="0740e-108">Käytä **Resurssienhallinta-näkymässä** .</span><span class="sxs-lookup"><span data-stu-id="0740e-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="0740e-109">Valitse **Näytä asetukset** \> **Resurssienhallinta-näkymässä**.</span><span class="sxs-lookup"><span data-stu-id="0740e-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="0740e-110">Resurssienhallinta-näkymässä ei ole yhteensopiva Microsoft Edge, Google Chrome, Firefox ja muut.</span><span class="sxs-lookup"><span data-stu-id="0740e-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="0740e-111">**Resurssienhallinta-näkymässä** käytettävissä vain Internet Explorerissa.</span><span class="sxs-lookup"><span data-stu-id="0740e-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="0740e-112">Varmista, että WebClient-palvelu on käynnissä.</span><span class="sxs-lookup"><span data-stu-id="0740e-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="0740e-113">Windows-hakuruutuun Suorita, tyyppi valitse Suorita desktop app, kirjoita services.msc ja paina sitten Enter.</span><span class="sxs-lookup"><span data-stu-id="0740e-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="0740e-114">WebClient-palvelua kohtaan ja varmista, että **tila** -sarakkeessa näkyy ”käynnissä”.</span><span class="sxs-lookup"><span data-stu-id="0740e-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="0740e-115">Jos näin ei ole, kaksoisnapsauta palvelua, napsauttamalla **Käynnistä-painiketta**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="0740e-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="0740e-116">(Saatat joutua ensin otettava palvelu käyttöön valitsemalla **manuaalisen** tai **automaattisen** **käynnistyksen tyyppi** -ruudusta.)</span><span class="sxs-lookup"><span data-stu-id="0740e-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="0740e-117">Kirjaston avaaminen Resurssienhallinta on kätevä, jos haluat kopioida tai siirtää useita tiedostoja ja kansioita, kun, mutta jos haluat käyttää säännöllisesti kirjastossa, suosittelemme synkronoit sen.</span><span class="sxs-lookup"><span data-stu-id="0740e-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="0740e-118">Avattaessa tiedostoa Explorer-ongelmien vianmäärityksen, on [avoinna Resurssienhallinnassa](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="0740e-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="0740e-119">Katso tiedot synkronoinnin määrittäminen [OneDrive synkronointi uuden asiakkaan kanssa synkronointi SharePoint-tiedostot](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="0740e-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="0740e-120">On lisätietoja artikkelissa [SharePoint Online-ongelmien vianmääritys ”Open kanssa Explorer”-komennon käyttämisestä](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) .</span><span class="sxs-lookup"><span data-stu-id="0740e-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

