---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770988"
---
# <a name="verify-your-domain"></a><span data-ttu-id="4ec88-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="4ec88-102">Verify your domain</span></span>

 <span data-ttu-id="4ec88-103">**Tietue ei todennäköisesti ole päivittunut Internetissä.**</span><span class="sxs-lookup"><span data-stu-id="4ec88-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="4ec88-104">Yleensä tietueen näkemiseen menee vain muutama minuutti, mutta välillä siihen saattaa kulua jopa pari tuntia.</span><span class="sxs-lookup"><span data-stu-id="4ec88-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="4ec88-105">Jos olet odottanut niin kauan, varmista, että olet kopioinut ja liitnyt täsmällisen arvon DNS-isännöintipalvelun TXT-vahvistustietueeseen.</span><span class="sxs-lookup"><span data-stu-id="4ec88-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="4ec88-106">Eräs yleinen virhe on unohtaa tietueen MS= -osa.</span><span class="sxs-lookup"><span data-stu-id="4ec88-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="4ec88-107">Sitäkin tarvitaan!</span><span class="sxs-lookup"><span data-stu-id="4ec88-107">We need that too!</span></span>

- <span data-ttu-id="4ec88-108">Joissain DNS-palvelimissa vyöhyketiedoston (johon DNS-tietue on tallennettu) tallentamiseen tarvitaan yksi ylimääräinen vaihe, jotta se päivittyy kaikkialle Internetiin.</span><span class="sxs-lookup"><span data-stu-id="4ec88-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="4ec88-109">Varmista, että olet tallentanut muutokset, jotta Microsoft voi tarkastella ja vahvistaa tietueen.</span><span class="sxs-lookup"><span data-stu-id="4ec88-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
