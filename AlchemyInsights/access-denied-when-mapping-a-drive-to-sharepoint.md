---
title: Käyttö estetty, kun asema yhdistettiin SharePointiin
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
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 23ee86df5404b6f20f3a4b605038b31b6f9fd731
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687363"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="26bbc-102">Verkkoasemiin yhdistettyjen SharePoint-kirjastojen ongelmien korjaaminen</span><span class="sxs-lookup"><span data-stu-id="26bbc-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="26bbc-103">Kun selaat yhdistettyä verkkoasemaa, saatat nähdä jonkin seuraavista sanomista:</span><span class="sxs-lookup"><span data-stu-id="26bbc-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="26bbc-104">**\\Polku ei ole käytettävissä. Sinulla ei ehkä ole tämän verkkoresurssin käyttöoikeuksia. Ota yhteyttä tämän palvelimen järjestelmänvalvojaan ja selvitä, onko sinulla käyttöoikeudet.**</span><span class="sxs-lookup"><span data-stu-id="26bbc-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="26bbc-105">**Käyttö estetty. Ennen kuin avaat tiedostoja tässä sijainnissa, sinun on ensin lisättävä web-sivusto luotettujen sivustoluetteloosi, siirryttävä web-sivustoon ja valittava mahdollisuus kirjautua automaattisesti sisään.**</span><span class="sxs-lookup"><span data-stu-id="26bbc-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="26bbc-106">[Ohjeita yhdistettyjen verkkoasemien vianmääritykseen](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="26bbc-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="26bbc-107">Kirjaston yhdistäminen verkkoasemaksi on tilapäistä, ja sitä tuetaan vain Internet Explorerissa.</span><span class="sxs-lookup"><span data-stu-id="26bbc-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="26bbc-108">Synkronoi sen sijaan [SharePoint-tiedostot uuden OneDrive-synkronointiohjelman kanssa,](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) joka sisältää [Files On-Demand -ohjelman.](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)</span><span class="sxs-lookup"><span data-stu-id="26bbc-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="26bbc-109">Käytä kaikkia Tiedostoja OneDrivessa käyttämättä paikallista tallennustilaa.</span><span class="sxs-lookup"><span data-stu-id="26bbc-109">Access all your files in OneDrive without using local storage space.</span></span>
  