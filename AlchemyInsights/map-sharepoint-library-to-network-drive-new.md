---
title: SharePoint-kirjaston yhdistäminen verkkoasemaan
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: ca5adee1c7f6d87a4d1cd0d7fac34e51948ce6b4
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/09/2019
ms.locfileid: "36269553"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a><span data-ttu-id="c387c-102">SharePoint-kirjaston yhdistäminen verkkoasemaan</span><span class="sxs-lookup"><span data-stu-id="c387c-102">Map a SharePoint library to a network drive</span></span>

<span data-ttu-id="c387c-103">Yhdistäminen verkkoasemaan kuin kirjastoon on väliaikainen ja tuetaan vain Internet Explorerin kautta.</span><span class="sxs-lookup"><span data-stu-id="c387c-103">Mapping a library as a network drive is temporary and supported only through Internet Explorer.</span></span> <span data-ttu-id="c387c-104">Joskus sinun täytyy SharePoint-sivuston avaaminen Internet Explorerissa ja valita estää istunto päättyy **Kun pysyt kirjautuneena** .</span><span class="sxs-lookup"><span data-stu-id="c387c-104">You must occasionally open the SharePoint site in Internet Explorer and select **Stay signed in** to prevent the session from expiring.</span></span> <span data-ttu-id="c387c-105">Sen sijaan [synkronoida SharePoint-tiedostot OneDrive synkronointi uuden asiakkaan kanssa](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) </a> joka tarjoaa [Tiedostot tarvittaessa](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span><span class="sxs-lookup"><span data-stu-id="c387c-105">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span></span> <span data-ttu-id="c387c-106">Kaikki OneDrive tiedostot käyttää ilman paikallista tallennustilaa.</span><span class="sxs-lookup"><span data-stu-id="c387c-106">Access all your files in OneDrive without using local storage space.</span></span>

<span data-ttu-id="c387c-107">Voit halutessasi yhdistää aseman sijaan [uuden OneDrive synkronointi-asiakas](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)varmistaa artikkelin ohjeita noudattamalla.</span><span class="sxs-lookup"><span data-stu-id="c387c-107">If you choose to map a drive instead of [using the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), ensure you follow the steps in the article below.</span></span> 


<span data-ttu-id="c387c-108">**Yhdistettyjen verkkoasemien määrittäminen ja vianmääritys**</span><span class="sxs-lookup"><span data-stu-id="c387c-108">**How to configure and troubleshoot mapped network drives**</span></span>


<span data-ttu-id="c387c-109">Katso [asetusten määrittäminen ja vianmääritys yhdistettyihin verkkoasemiin](https://support.office.com/article/troubleshoot-mapped-network-drives-that-connect-to-sharepoint-online-ef399c67-4578-4c3a-adbe-0b489084eabe?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="c387c-109">See [Configure and to troubleshoot mapped network drives](https://support.office.com/article/troubleshoot-mapped-network-drives-that-connect-to-sharepoint-online-ef399c67-4578-4c3a-adbe-0b489084eabe?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

<span data-ttu-id="c387c-110">Huomautus: Jos käyttää Internet Explorer 10 Windows 8 ja Windows 7: n kanssa, ja tulla **käyttö estetty** tai **polku ei ole käytettävissä** , kun yhdistät aseman asentaa [tämän hotfix-korjauksen](https://support.microsoft.com/help/2846960) tämän ongelman ratkaisemiseksi.</span><span class="sxs-lookup"><span data-stu-id="c387c-110">NOTE:  If you use Internet Explorer 10 with Windows 8 or Windows 7, and receive **Access denied** or **Path is not accessible** when mapping a drive, install [this hotfix](https://support.microsoft.com/help/2846960) to resolve this problem.</span></span> 
