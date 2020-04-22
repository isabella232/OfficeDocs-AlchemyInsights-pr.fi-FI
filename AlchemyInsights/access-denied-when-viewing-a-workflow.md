---
title: Käyttö estetty työnkulun tarkastelemisen yhteydessä
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687327"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="52166-102">Käyttö estetty työnkulun tarkastelemisen yhteydessä</span><span class="sxs-lookup"><span data-stu-id="52166-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="52166-103">SharePoint 2013 -työnkulut, jotka yrittävät lähettää sähköpostia SharePoint-ryhmään, voivat epäonnistua Käyttö estetty -virhesanoman kanssa, jos SharePoint-ryhmän jäsenyyden arvoksi ei ole määritetty Kaikki.</span><span class="sxs-lookup"><span data-stu-id="52166-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="52166-104">**Voit ratkaista tämän ongelman seuraavasti:**</span><span class="sxs-lookup"><span data-stu-id="52166-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="52166-105">Salli kaikkien nähdä SharePoint-ryhmän jäsenet.</span><span class="sxs-lookup"><span data-stu-id="52166-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="52166-106">Poista SharePoint-ryhmä sähköpostin Vastaanottaja- tai Kopio-riviltä.</span><span class="sxs-lookup"><span data-stu-id="52166-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="52166-107">Lisää käyttäjät erikseen Vastaanottaja- tai Kopio-riville, jos jäsenyyden näkyvyyttä ei voi muuttaa SharePoint-ryhmässä.</span><span class="sxs-lookup"><span data-stu-id="52166-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="52166-108">Lisätietoja on [http:ssä http:n luvaton http-tiedoston /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="52166-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  