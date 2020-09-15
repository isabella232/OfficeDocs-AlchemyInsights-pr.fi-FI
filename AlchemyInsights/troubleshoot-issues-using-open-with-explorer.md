---
title: Avaa Resurssienhallinnassa-toiminnon ongelmien vian määritys
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659055"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="3a718-102">Avaa Resurssienhallinnassa-ongelmien korjaaminen</span><span class="sxs-lookup"><span data-stu-id="3a718-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="3a718-103">Yleisten ongelmien korjaaminen avaamalla tiedosto Kirjasto SharePointissa tai OneDrivessa **Avaa Resurssienhallinnassa-** komennon avulla:</span><span class="sxs-lookup"><span data-stu-id="3a718-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="3a718-104">Käytä Internet Explorer 10: tä tai Internet Explorer 11-ohjelmistoa.</span><span class="sxs-lookup"><span data-stu-id="3a718-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="3a718-105">**Avaa Resurssienhallinnassa** ei ole yhteensopiva Microsoft Edgessä, Google Chromessa, Firefoxissa ja muissa.</span><span class="sxs-lookup"><span data-stu-id="3a718-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="3a718-106">**Avaa Resurssienhallinnassa** ei ole käytössä kaikissa selaimissa paitsi Internet Explorerissa.</span><span class="sxs-lookup"><span data-stu-id="3a718-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="3a718-107">**Avaa Resurssienhallinnassa-** toiminto ei ole käytettävissä SharePoint-kirjastojen nykyaikaisessa käyttö kokemuksessa.</span><span class="sxs-lookup"><span data-stu-id="3a718-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="3a718-108">Käytä **Näytä Resurssienhallinnassa-** komentoa.</span><span class="sxs-lookup"><span data-stu-id="3a718-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="3a718-109">Valitse **Näytä asetukset** \> **-näkymä Resurssienhallinnassa**.</span><span class="sxs-lookup"><span data-stu-id="3a718-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="3a718-110">Näytä Resurssienhallinnassa ei ole yhteensopiva Microsoft Edgessä, Google Chromessa, Firefoxissa ja muissa.</span><span class="sxs-lookup"><span data-stu-id="3a718-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="3a718-111">**Näytä Resurssienhallinnassa** -kohdassa käytettävissä vain Internet Explorerissa.</span><span class="sxs-lookup"><span data-stu-id="3a718-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="3a718-112">Varmista, että WebClient-palvelu on käynnissä.</span><span class="sxs-lookup"><span data-stu-id="3a718-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="3a718-113">Kirjoita Windowsin haku ruutuun Suorita, valitse Suorita Työpöytä sovellus, kirjoita Services. msc ja paina sitten ENTER-näppäintä.</span><span class="sxs-lookup"><span data-stu-id="3a718-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="3a718-114">Vieritä alas WebClient-palveluun ja varmista, että **tila** -sarakkeessa lukee "Running".</span><span class="sxs-lookup"><span data-stu-id="3a718-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="3a718-115">Jos se ei onnistu, kaksoisnapsauta palvelua, valitse **Käynnistä**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="3a718-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="3a718-116">(Sinun on ehkä ensin otettava palvelu käyttöön valitsemalla **Käynnistys tapa** -ruudussa joko **Manuaalinen** tai **Automaattinen** .)</span><span class="sxs-lookup"><span data-stu-id="3a718-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="3a718-117">Kirjaston avaaminen Resurssienhallinnassa on kätevää, jos sinun täytyy kopioida tai siirtää useita tiedostoja ja kansioita kerran, mutta jos haluat työskennellä kirjastossa säännöllisesti, suosittelemme sen synkronointia.</span><span class="sxs-lookup"><span data-stu-id="3a718-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="3a718-118">Lisä tietoja Resurssienhallinnan avaamis ongelmien vian määrityksestä on kohdassa [Avaa Resurssienhallinnassa](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="3a718-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="3a718-119">Lisä tietoja synkronoinnin määrittämisestä on Ohje aiheessa [SharePoint-tiedostojen synkronointi uuden OneDrive-synkronointi sovelluksen avulla](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="3a718-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="3a718-120">Katso lisä tietoja artikkelista [Avaa Resurssienhallinnassa-komennon käyttäminen SharePoint Onlinen ongelmien vian määrityksessä](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) .</span><span class="sxs-lookup"><span data-stu-id="3a718-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

