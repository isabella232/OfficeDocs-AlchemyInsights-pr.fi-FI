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
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36747745"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Käyttö estetty työn kulkua tarkasteltaessa

SharePoint 2013-työn kulut, jotka yrittävät lähettää sähkö postia SharePoint-ryhmään, voivat epäonnistua käyttö estetty-virhe sanomassa, jos SharePoint-ryhmän jäsenyyttä ei ole määritetty kaikille.
  
 **Voit ratkaista tämän ongelman tekemällä seuraavat toimet:**
  
 1. Salli kaikkien nähdä SharePoint-ryhmän jäsenet.
  
 2. Poista SharePoint-ryhmä Sähkö posti viestin to-tai CC-riviltä.
  
 3. Lisää käyttäjät eksplisiittisesti to-tai CC-riville, jos SharePoint-ryhmän jäsenyyden näkyvyyttä ei voi muuttaa.
  
Katso lisä tietoja kohdasta [http luvaton/_vti_bin/Client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  