---
title: Käyttö estetty, kun asema yhdistetään SharePointiin
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: c41bfd9d25c8aa946a4ec5156be6d2424f4e2133
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737474"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="08e4a-102">Verkko asemiin yhdistettyjen SharePoint-kirjastojen ongelmien korjaaminen</span><span class="sxs-lookup"><span data-stu-id="08e4a-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="08e4a-103">Kun selaat yhdistettyä verkko asemaa, saatat nähdä jonkin seuraavista viesteistä:</span><span class="sxs-lookup"><span data-stu-id="08e4a-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="08e4a-104">**\\Polku ei ole käytettävissä. Sinulla ei ehkä ole tämän verkko resurssin käyttö oikeutta. Ota yhteyttä tämän palvelimen järjestelmänvalvojaan ja selvitä, onko sinulla käyttö oikeudet.**</span><span class="sxs-lookup"><span data-stu-id="08e4a-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="08e4a-105">**Käyttö estetty. Ennen kuin avaat tässä sijainnissa olevat tiedostot, sinun on ensin lisättävä Web-sivusto luotettujen sivustojen luetteloon, selaamalla Web-sivustoon ja valitsemalla vaihto ehto Kirjaudu automaattisesti sisään.**</span><span class="sxs-lookup"><span data-stu-id="08e4a-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="08e4a-106">[Hanki ohjeita yhdistettyjen verkko asemien vian määritykseen](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="08e4a-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="08e4a-107">Kirjaston yhdistäminen verkko asemiksi on väliaikaista ja sitä tuetaan vain Internet Explorerissa.</span><span class="sxs-lookup"><span data-stu-id="08e4a-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="08e4a-108">Synkronoi sen sijaan [SharePoint-tiedostot uudella OneDrive-synkronointi ohjelmalla](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) , joka sisältää [tiedostot](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)pyydettäessä.</span><span class="sxs-lookup"><span data-stu-id="08e4a-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="08e4a-109">Käyttää kaikkia tiedostojasi OneDrivessa ilman paikallista tallennus tilaa.</span><span class="sxs-lookup"><span data-stu-id="08e4a-109">Access all your files in OneDrive without using local storage space.</span></span>
  