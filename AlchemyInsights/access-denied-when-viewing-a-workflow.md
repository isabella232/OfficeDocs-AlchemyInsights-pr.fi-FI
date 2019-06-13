---
title: Käyttö on estetty, kun tarkastelet työnkulun
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: b7a3805d30cac44781adbbb00c0f0ed3496ff17b
ms.sourcegitcommit: a9be2e396022382e92cf40c0d0d82f2f59c2e259
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/12/2019
ms.locfileid: "34883588"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="3a2ed-102">Käyttö on estetty, kun tarkastelet työnkulun</span><span class="sxs-lookup"><span data-stu-id="3a2ed-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="3a2ed-103">SharePoint-2013 työnkulkuja, jotka yrittävät lähettää sähköpostia SharePoint-ryhmään voi epäonnistua ”käyttö estetty”-virhesanoman, jos SharePoint-ryhmän jäsenyys ei ole kaikille.</span><span class="sxs-lookup"><span data-stu-id="3a2ed-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="3a2ed-104">**Voit ratkaista tämän ongelman, toimi seuraavasti:**</span><span class="sxs-lookup"><span data-stu-id="3a2ed-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="3a2ed-105">Salli kaikki SharePoint-ryhmän jäsenillä on.</span><span class="sxs-lookup"><span data-stu-id="3a2ed-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="3a2ed-106">Poista SharePoint-ryhmän vastaanottaja- tai Kopio-rivi sähköpostiviestin.</span><span class="sxs-lookup"><span data-stu-id="3a2ed-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="3a2ed-107">Lisätä käyttäjiä suoraan vastaanottaja- tai Kopio rivi, jos SharePoint-ryhmän jäsenyyden näkyvyyttä ei voi muuttaa.</span><span class="sxs-lookup"><span data-stu-id="3a2ed-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="3a2ed-108">Saat lisätietoja Tutustu [/_vti_bin/client.svc/sp.utilities.utility.SendEmail luvattoman HTTP](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="3a2ed-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  