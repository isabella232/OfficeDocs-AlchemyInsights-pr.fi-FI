---
title: Käyttö estetty tarkasteltaessa työn kulkua
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688799"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Käyttö estetty tarkasteltaessa työn kulkua

SharePoint 2013-työn kulut, jotka yrittävät lähettää sähkö postia SharePoint-ryhmälle, voivat epäonnistua käyttö estetty-virhe sanomassa, jos SharePoint-ryhmän jäsenyyttä ei ole valittu kaikille.
  
 **Voit korjata ongelman toimimalla seuraavasti:**
  
 1. Salli kaikkien nähdä SharePoint-ryhmän jäsenet.
  
 2. Poista SharePoint-ryhmä Sähkö posti viestin vastaanottaja-tai kopio-riviltä.
  
 3. Lisää käyttäjät suoraan vastaanottaja-tai kopio-riville, jos SharePoint-ryhmän jäsenyyden näkyvyyttä ei voi muuttaa.
  
Jos haluat lisä tietoja, katso [HTTP _vti_bin/Client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  