---
title: Käyttö estetty työn kulkua tarkasteltaessa
ms.author: pebaum
author: pebaum
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 1cfda8e08ada05858a28f2bede8c31261f9de351
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050522"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="cdabc-102">Käyttö estetty työn kulkua tarkasteltaessa</span><span class="sxs-lookup"><span data-stu-id="cdabc-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="cdabc-103">SharePoint 2013-työn kulut, jotka yrittävät lähettää sähkö postia SharePoint-ryhmään, voivat epäonnistua käyttö estetty-virhe sanomassa, jos SharePoint-ryhmän jäsenyyttä ei ole määritetty kaikille.</span><span class="sxs-lookup"><span data-stu-id="cdabc-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="cdabc-104">**Voit ratkaista tämän ongelman tekemällä seuraavat toimet:**</span><span class="sxs-lookup"><span data-stu-id="cdabc-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="cdabc-105">Salli kaikkien nähdä SharePoint-ryhmän jäsenet.</span><span class="sxs-lookup"><span data-stu-id="cdabc-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="cdabc-106">Poista SharePoint-ryhmä Sähkö posti viestin to-tai CC-riviltä.</span><span class="sxs-lookup"><span data-stu-id="cdabc-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="cdabc-107">Lisää käyttäjät eksplisiittisesti to-tai CC-riville, jos SharePoint-ryhmän jäsenyyden näkyvyyttä ei voi muuttaa.</span><span class="sxs-lookup"><span data-stu-id="cdabc-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="cdabc-108">Katso lisä tietoja kohdasta [http luvaton/_vti_bin/Client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="cdabc-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  