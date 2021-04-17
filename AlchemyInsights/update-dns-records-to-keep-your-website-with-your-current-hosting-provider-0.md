---
title: DNS-tietueiden päivittäminen sivuston säilyttämiseksi nykyisessä isännöintipalvelussa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827512"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="4a1cf-102">DNS-tietueiden päivittäminen sivuston säilyttämiseksi nykyisessä isännöintipalvelussa</span><span class="sxs-lookup"><span data-stu-id="4a1cf-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="4a1cf-103">Siirry Microsoft 365 -hallintakeskuksessa Määritä toimialueet -sivulle ja valitse toimialueiden luettelosta toimialue, jossa käytät  >  [](https://admin.microsoft.com/Adminportal#/Domains) sivustoasi.</span><span class="sxs-lookup"><span data-stu-id="4a1cf-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="4a1cf-104">Valitse **+ Uusi mukautettu tietue** ja anna seuraavat tiedot:</span><span class="sxs-lookup"><span data-stu-id="4a1cf-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="4a1cf-105">Määritä **DNS-tyyppi**: **A (osoite)**</span><span class="sxs-lookup"><span data-stu-id="4a1cf-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="4a1cf-106">Kirjoita **Isäntänimi tai alias** -kohtaan **@**</span><span class="sxs-lookup"><span data-stu-id="4a1cf-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="4a1cf-107">Kirjoita **IP-osoite** -kohtaan muualla isännöidyn sivustosi staattinen IP-osoite, esimerkiksi 172.16.140.1.</span><span class="sxs-lookup"><span data-stu-id="4a1cf-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="4a1cf-p101">Sivuston osoitteen on oltava  *staattinen*  IP-osoite, ei  *dynaaminen*  IP-osoite. Tarkista sivustosi isännöintipalvelusta, voitko saada käyttöön staattisen IP-osoitteen julkista sivustoasi varten.</span><span class="sxs-lookup"><span data-stu-id="4a1cf-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="4a1cf-110">Valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="4a1cf-110">Select **Save**.</span></span>

<span data-ttu-id="4a1cf-111">Voit halutessasi luoda myös CNAME-tietueen, joka auttaa asiakkaita löytämään sivuston.</span><span class="sxs-lookup"><span data-stu-id="4a1cf-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="4a1cf-112">Valitse **+ Uusi mukautettu tietue** ja anna seuraavat tiedot:</span><span class="sxs-lookup"><span data-stu-id="4a1cf-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="4a1cf-113">Määritä **DNS-tyyppi**: **CNAME (alias)**</span><span class="sxs-lookup"><span data-stu-id="4a1cf-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="4a1cf-114">Kirjoita **Isäntänimi tai alias** -kohtaan **www**</span><span class="sxs-lookup"><span data-stu-id="4a1cf-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="4a1cf-115">Kirjoita **Kohdeosoite** -kohtaan sivuston täydellinen toimialuenimi, esimerkiksi contoso.com.</span><span class="sxs-lookup"><span data-stu-id="4a1cf-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="4a1cf-116">Valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="4a1cf-116">Select **Save**.</span></span>
