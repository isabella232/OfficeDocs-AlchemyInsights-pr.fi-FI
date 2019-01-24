---
title: DNS-tietueiden päivittäminen sivuston säilyttämiseksi nykyisessä isännöintipalvelussa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29467638"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="c7b58-102">DNS-tietueiden päivittäminen sivuston säilyttämiseksi nykyisessä isännöintipalvelussa</span><span class="sxs-lookup"><span data-stu-id="c7b58-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="c7b58-103">Valitse [Toimialueet](https://portal.office.com/adminportal/home#/Domains) -sivun luettelosta toimialue, jota käytät sivustossasi. Valitse sitten **DNS-asetukset** hallintaruudussa.</span><span class="sxs-lookup"><span data-stu-id="c7b58-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="c7b58-104">Valitse **+ Uusi mukautettu tietue** ja anna seuraavat tiedot:</span><span class="sxs-lookup"><span data-stu-id="c7b58-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="c7b58-105">Määritä **DNS-tyyppi**: **A (osoite)**</span><span class="sxs-lookup"><span data-stu-id="c7b58-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="c7b58-106">Kirjoita **Isäntänimi tai alias** -kohtaan **@**</span><span class="sxs-lookup"><span data-stu-id="c7b58-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="c7b58-107">Kirjoita **IP-osoite** -kohtaan muualla isännöidyn sivustosi staattinen IP-osoite, esimerkiksi 172.16.140.1.</span><span class="sxs-lookup"><span data-stu-id="c7b58-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="c7b58-p101">Sivuston osoitteen on oltava  *staattinen*  IP-osoite, ei  *dynaaminen*  IP-osoite. Tarkista sivustosi isännöintipalvelusta, voitko saada käyttöön staattisen IP-osoitteen julkista sivustoasi varten.</span><span class="sxs-lookup"><span data-stu-id="c7b58-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="c7b58-110">Valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="c7b58-110">Select **Save**.</span></span> 
    
<span data-ttu-id="c7b58-111">Voit halutessasi luoda myös CNAME-tietueen, joka auttaa asiakkaita löytämään sivuston.</span><span class="sxs-lookup"><span data-stu-id="c7b58-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="c7b58-112">Valitse **+ Uusi mukautettu tietue** ja anna seuraavat tiedot:</span><span class="sxs-lookup"><span data-stu-id="c7b58-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="c7b58-113">Määritä **DNS-tyyppi**: **CNAME (alias)**</span><span class="sxs-lookup"><span data-stu-id="c7b58-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="c7b58-114">Kirjoita **Isäntänimi tai alias** -kohtaan **www**</span><span class="sxs-lookup"><span data-stu-id="c7b58-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="c7b58-115">Kirjoita **Kohdeosoite** -kohtaan sivuston täydellinen toimialuenimi, esimerkiksi contoso.com.</span><span class="sxs-lookup"><span data-stu-id="c7b58-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="c7b58-116">Valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="c7b58-116">Select **Save**.</span></span> 
    

