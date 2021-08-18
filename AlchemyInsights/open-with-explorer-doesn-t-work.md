---
title: Avaa Resurssienhallinnassa -tiedosto ei toimi
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 2ba6f08b40dd194bf1ffd9a455a134a2fc553b51
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321858"
---
# <a name="open-with-explorer-isnt-working"></a>Avaa Resurssienhallinnassa -käyttö ei toimi

Jos **Avaa Resurssienhallinnassa-** tai Näytä **Resurssienhallinnassa** -komento ei toimi,  varmista, että WebClient-palvelun arvoksi on määritetty Käynnissä alla olevia ohjeita noudattamalla. Esimerkiksi kirjaston tai kirjaston SharePoint OneDrive, kun palvelu ei ole käynnissä, saattaa kestää kauan. 
  
1. Kirjoita Windows-ruutuun suorita, valitse Suorita työpöytäsovellus, kirjoita services.msc ja valitse sitten **Enter**.
    
2. Vieritä alaspäin WEBClient-palveluun ja valitse **Tila-sarake.** Jos WWW-asiakassovelluksen palvelun tila ei **ole Käynnissä**, kaksoisnapsauta palvelua, valitse **Käynnistä** ja valitse sitten **OK**. Ota palvelu tarvittaessa käyttöön valitsemalla **Käynnistystapa-ruudussa** **joko** Manuaalinen **tai** Automaattinen. 
    
**Huomautus:** Lisätietoja Resurssienhallinnan avaamisen vianmäärityksestä on ohjeaiheessa [Avaa Resurssienhallinnassa.](https://go.microsoft.com/fwlink/?linkid=871665) Tutustu synkronointiin paremmana vaihtoehtona: [synkronoi SharePoint uuden OneDrive-synkronointisovellus kanssa.](https://go.microsoft.com/fwlink/?linkid=871666) 
  

