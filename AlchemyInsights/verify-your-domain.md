---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 2c4d8e075d2cf7214b5ef005b856daf7fb0ed53c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710440"
---
# <a name="verify-your-domain"></a><span data-ttu-id="4f658-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="4f658-102">Verify your domain</span></span>

 <span data-ttu-id="4f658-103">**Tietuetta ei todennäköisesti ole päivitetty Internetissä.**</span><span class="sxs-lookup"><span data-stu-id="4f658-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="4f658-104">Yleensä tietueen näkemiseen menee vain muutama minuutti, mutta välillä siihen saattaa kulua jopa pari tuntia.</span><span class="sxs-lookup"><span data-stu-id="4f658-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="4f658-105">Jos olet odottanut niin kauan jo, tarkista, että olet kopioinut ja liittänyt tarkan arvon TXT-vahvistustietueeseen DNS-isännässäsi.</span><span class="sxs-lookup"><span data-stu-id="4f658-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="4f658-106">Eräs yleinen virhe on unohtaa tietueen MS= -osa.</span><span class="sxs-lookup"><span data-stu-id="4f658-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="4f658-107">Sitäkin tarvitaan!</span><span class="sxs-lookup"><span data-stu-id="4f658-107">We need that too!</span></span>

- <span data-ttu-id="4f658-108">Joissain DNS-palvelimissa vyöhyketiedoston (johon DNS-tietue on tallennettu) tallentamiseen tarvitaan yksi ylimääräinen vaihe, jotta se päivittyy kaikkialle Internetiin.</span><span class="sxs-lookup"><span data-stu-id="4f658-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="4f658-109">Varmista, että olet tallentanut muutokset, jotta Microsoft voi tarkastella ja vahvistaa tietueen.</span><span class="sxs-lookup"><span data-stu-id="4f658-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
