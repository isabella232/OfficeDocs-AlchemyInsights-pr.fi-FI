---
title: DNS-tietueiden päivittäminen sivuston säilyttämiseksi nykyisessä isännöintipalvelussa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a1ea0589def4945da64c73d68b2e4a3d64d6b83d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506404"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="fc03a-102">DNS-tietueiden päivittäminen sivuston säilyttämiseksi nykyisessä isännöintipalvelussa</span><span class="sxs-lookup"><span data-stu-id="fc03a-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="fc03a-103">Valitse [Domains](https://portal.office.com/adminportal/home#/Domains) -sivun toimialueluetteloa, käytät Web-sivuston toimialueen.</span><span class="sxs-lookup"><span data-stu-id="fc03a-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="fc03a-104">Valitse **+ Uusi mukautettu tietue** ja anna seuraavat tiedot:</span><span class="sxs-lookup"><span data-stu-id="fc03a-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="fc03a-105">Määritä **DNS-tyyppi**: **A (osoite)**</span><span class="sxs-lookup"><span data-stu-id="fc03a-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="fc03a-106">Kirjoita **Isäntänimi tai alias** -kohtaan **@**</span><span class="sxs-lookup"><span data-stu-id="fc03a-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="fc03a-107">Kirjoita **IP-osoite** -kohtaan muualla isännöidyn sivustosi staattinen IP-osoite, esimerkiksi 172.16.140.1.</span><span class="sxs-lookup"><span data-stu-id="fc03a-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="fc03a-p101">Sivuston osoitteen on oltava  *staattinen*  IP-osoite, ei  *dynaaminen*  IP-osoite. Tarkista sivustosi isännöintipalvelusta, voitko saada käyttöön staattisen IP-osoitteen julkista sivustoasi varten.</span><span class="sxs-lookup"><span data-stu-id="fc03a-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="fc03a-110">Valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="fc03a-110">Select **Save**.</span></span>

<span data-ttu-id="fc03a-111">Voit halutessasi luoda myös CNAME-tietueen, joka auttaa asiakkaita löytämään sivuston.</span><span class="sxs-lookup"><span data-stu-id="fc03a-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="fc03a-112">Valitse **+ Uusi mukautettu tietue** ja anna seuraavat tiedot:</span><span class="sxs-lookup"><span data-stu-id="fc03a-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="fc03a-113">Määritä **DNS-tyyppi**: **CNAME (alias)**</span><span class="sxs-lookup"><span data-stu-id="fc03a-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="fc03a-114">Kirjoita **Isäntänimi tai alias** -kohtaan **www**</span><span class="sxs-lookup"><span data-stu-id="fc03a-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="fc03a-115">Kirjoita **Kohdeosoite** -kohtaan sivuston täydellinen toimialuenimi, esimerkiksi contoso.com.</span><span class="sxs-lookup"><span data-stu-id="fc03a-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="fc03a-116">Valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="fc03a-116">Select **Save**.</span></span>
