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
ms.custom: Adm_O365
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 9b2abe01a47d39812988d62b6f010a8933fad33e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29929199"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="c8d85-102">Avaa Explorer liittyvien ongelmien korjaaminen</span><span class="sxs-lookup"><span data-stu-id="c8d85-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="c8d85-103">Yleisten ongelmien avaamalla asiakirjakirjaston SharePoint- tai OneDrive **Avaa Explorerissa** -komennolla:</span><span class="sxs-lookup"><span data-stu-id="c8d85-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="c8d85-p101">Käytä Internet Explorer 10 tai Internet Explorerin 11. **Avaa Explorerissa** ei ole yhteensopiva Microsoft Edge, Google Chrome, Firefox ja muut. **Avaa Explorerissa** ei ole käytettävissä kaikissa selaimissa kuin Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="c8d85-p101">Use Internet Explorer 10 or Internet Explorer 11. **Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others. **Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="c8d85-p102">**Avaa Explorerissa** ei ole käytettävissä SharePoint-kirjastoihin, Moderni kokemus. Käytä **Resurssienhallinta-näkymässä** . Valitse **Näytä asetukset** \> **Resurssienhallinta-näkymässä**. Resurssienhallinta-näkymässä ei ole yhteensopiva Microsoft Edge, Google Chrome, Firefox ja muut. **Resurssienhallinta-näkymässä** käytettävissä vain Internet Explorerissa.</span><span class="sxs-lookup"><span data-stu-id="c8d85-p102">**Open with Explorer** is not available in the modern experience for SharePoint libraries. Use **View in File Explorer** instead. Select **View options** \> **View in File Explorer**. View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others. **View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="c8d85-p103">Varmista, että WebClient-palvelu on käynnissä. Windows-hakuruutuun Suorita, tyyppi valitse Suorita desktop app, kirjoita services.msc ja paina sitten Enter. WebClient-palvelua kohtaan ja varmista, että **tila** -sarakkeessa näkyy ”käynnissä”. Jos näin ei ole, kaksoisnapsauta palvelua, napsauttamalla **Käynnistä-painiketta**ja valitse sitten **OK**. (Saatat joutua ensin otettava palvelu käyttöön valitsemalla **manuaalisen** tai **automaattisen** **käynnistyksen tyyppi** -ruudusta.)</span><span class="sxs-lookup"><span data-stu-id="c8d85-p103">Make sure the WebClient service is running. In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter. Scroll down to the WebClient service and make sure the **Status** column displays "Running." If it doesn't, double-click the service, click **Start**, and then click **OK**. (You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="c8d85-p104">Kirjaston avaaminen Resurssienhallinta on kätevä, jos haluat kopioida tai siirtää useita tiedostoja ja kansioita, kun, mutta jos haluat käyttää säännöllisesti kirjastossa, suosittelemme synkronoit sen. Avattaessa tiedostoa Explorer-ongelmien vianmäärityksen, on [avoinna Resurssienhallinnassa](https://go.microsoft.com/fwlink/?linkid=871665). Katso tiedot synkronoinnin määrittäminen [OneDrive synkronointi uuden asiakkaan kanssa synkronointi SharePoint-tiedostot](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="c8d85-p104">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it. To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="c8d85-120">On lisätietoja artikkelissa [SharePoint Online-ongelmien vianmääritys ”Open kanssa Explorer”-komennon käyttämisestä](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) .</span><span class="sxs-lookup"><span data-stu-id="c8d85-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

