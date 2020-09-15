---
title: Käyttö estetty, kun asema yhdistetään SharePointiin
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
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 8fc866390d63443c94beef76b6a53a628b85d6d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668740"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="7502f-102">Verkko asemiin yhdistettyjen SharePoint-kirjastojen ongelmien korjaaminen</span><span class="sxs-lookup"><span data-stu-id="7502f-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="7502f-103">Kun selaat yhdistettyyn verkko asemaan, näyttöön voi tulla jokin seuraavista viesteistä:</span><span class="sxs-lookup"><span data-stu-id="7502f-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="7502f-104">**\\Polku ei ole käytettävissä. Sinulla ei ehkä ole tämän verkko resurssin käyttö oikeutta. Ota yhteyttä tämän palvelimen järjestelmänvalvojaan ja selvitä, onko sinulla käyttö oikeudet.**</span><span class="sxs-lookup"><span data-stu-id="7502f-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="7502f-105">**Käyttö estetty. Ennen kuin avaat tämän sijainnin tiedostot, sinun on ensin lisättävä sivusto luotettujen sivustojen luetteloon, selaamalla sivustoon ja valitsemalla Automaattinen kirjautuminen-vaihto ehto.**</span><span class="sxs-lookup"><span data-stu-id="7502f-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="7502f-106">[Ohjeita yhdistettyjen verkko asemien vian määritykseen](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="7502f-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="7502f-107">Kirjaston määrittäminen verkko asemaksi on väliaikaista ja sitä tuetaan vain Internet Explorerissa.</span><span class="sxs-lookup"><span data-stu-id="7502f-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="7502f-108">Sen sijaan [Synkronoi SharePoint-tiedostot uuden OneDrive-synkronointi sovelluksen kanssa](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) , joka sisältää [tiedostoja pyydettäessä](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span><span class="sxs-lookup"><span data-stu-id="7502f-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="7502f-109">Käytä kaikkia tiedostojasi OneDrivessa käyttämättä paikallista tallennus tilaa.</span><span class="sxs-lookup"><span data-stu-id="7502f-109">Access all your files in OneDrive without using local storage space.</span></span>
  