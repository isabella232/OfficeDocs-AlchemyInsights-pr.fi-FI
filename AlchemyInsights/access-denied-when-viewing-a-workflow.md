---
title: Käyttö estetty työn kulkua tarkasteltaessa
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/15/2019
ms.locfileid: "36747745"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="d9dbd-102">Käyttö estetty työn kulkua tarkasteltaessa</span><span class="sxs-lookup"><span data-stu-id="d9dbd-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="d9dbd-103">SharePoint 2013-työn kulut, jotka yrittävät lähettää sähkö postia SharePoint-ryhmään, voivat epäonnistua käyttö estetty-virhe sanomassa, jos SharePoint-ryhmän jäsenyyttä ei ole määritetty kaikille.</span><span class="sxs-lookup"><span data-stu-id="d9dbd-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="d9dbd-104">**Voit ratkaista tämän ongelman tekemällä seuraavat toimet:**</span><span class="sxs-lookup"><span data-stu-id="d9dbd-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="d9dbd-105">Salli kaikkien nähdä SharePoint-ryhmän jäsenet.</span><span class="sxs-lookup"><span data-stu-id="d9dbd-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="d9dbd-106">Poista SharePoint-ryhmä Sähkö posti viestin to-tai CC-riviltä.</span><span class="sxs-lookup"><span data-stu-id="d9dbd-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="d9dbd-107">Lisää käyttäjät eksplisiittisesti to-tai CC-riville, jos SharePoint-ryhmän jäsenyyden näkyvyyttä ei voi muuttaa.</span><span class="sxs-lookup"><span data-stu-id="d9dbd-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="d9dbd-108">Katso lisä tietoja kohdasta [http luvaton/_vti_bin/Client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="d9dbd-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  