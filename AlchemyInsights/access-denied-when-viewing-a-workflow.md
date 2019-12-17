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
# <a name="access-denied-when-viewing-a-workflow"></a>Käyttö estetty työn kulkua tarkasteltaessa

SharePoint 2013-työn kulut, jotka yrittävät lähettää sähkö postia SharePoint-ryhmään, voivat epäonnistua käyttö estetty-virhe sanomassa, jos SharePoint-ryhmän jäsenyyttä ei ole määritetty kaikille.
  
 **Voit ratkaista tämän ongelman tekemällä seuraavat toimet:**
  
 1. Salli kaikkien nähdä SharePoint-ryhmän jäsenet.
  
 2. Poista SharePoint-ryhmä Sähkö posti viestin to-tai CC-riviltä.
  
 3. Lisää käyttäjät eksplisiittisesti to-tai CC-riville, jos SharePoint-ryhmän jäsenyyden näkyvyyttä ei voi muuttaa.
  
Katso lisä tietoja kohdasta [http luvaton/_vti_bin/Client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  