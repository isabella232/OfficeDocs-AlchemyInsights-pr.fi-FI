---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d215f3af0cf4b46b12c8cb51a9572adb00f354e4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420049"
---
# <a name="verify-your-domain"></a><span data-ttu-id="45e75-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="45e75-102">Verify your domain</span></span>

 <span data-ttu-id="45e75-103">**Tietueen luultavasti ei ole vielä päivitetty Internetin välityksellä.**</span><span class="sxs-lookup"><span data-stu-id="45e75-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="45e75-104">Yleensä tietueen näkemiseen menee vain muutama minuutti, mutta välillä siihen saattaa kulua jopa pari tuntia.</span><span class="sxs-lookup"><span data-stu-id="45e75-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="45e75-105">Tarkista, että olet odotti jo pitkään, jos olet kopioida ja liittää tarkka arvo TXT tarkastus-tietue DNS-isäntään.</span><span class="sxs-lookup"><span data-stu-id="45e75-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="45e75-106">Eräs yleinen virhe on unohtaa tietueen MS= -osa.</span><span class="sxs-lookup"><span data-stu-id="45e75-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="45e75-107">Sitäkin tarvitaan!</span><span class="sxs-lookup"><span data-stu-id="45e75-107">We need that too!</span></span>
    
- <span data-ttu-id="45e75-108">Joissain DNS-palvelimissa vyöhyketiedoston (johon DNS-tietue on tallennettu) tallentamiseen tarvitaan yksi ylimääräinen vaihe, jotta se päivittyy kaikkialle Internetiin.</span><span class="sxs-lookup"><span data-stu-id="45e75-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="45e75-109">Varmista, että olet tallentanut muutokset niin, että Office 365 näkee ja pystyy tarkistamaan tietueen.</span><span class="sxs-lookup"><span data-stu-id="45e75-109">Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
    

