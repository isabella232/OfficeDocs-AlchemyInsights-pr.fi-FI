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
ms.openlocfilehash: 164d5fe8c992df825d1f52f19792e1623526c35c58ff2f1e1ab601fdcf5f0f53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011333"
---
# <a name="open-with-explorer-isnt-working"></a>Avaa Resurssienhallinnassa -käyttö ei toimi

Jos **Avaa Resurssienhallinnassa-** tai Näytä **Resurssienhallinnassa** -komento ei toimi,  varmista, että WebClient-palvelun arvoksi on määritetty Käynnissä alla olevia ohjeita noudattamalla. Esimerkiksi kirjaston tai kirjaston SharePoint OneDrive, kun palvelu ei ole käynnissä, saattaa kestää kauan. 
  
1. Kirjoita Windows-ruutuun suorita, valitse Suorita työpöytäsovellus, kirjoita services.msc ja valitse sitten **Enter**.
    
2. Vieritä alaspäin WEBClient-palveluun ja valitse **Tila-sarake.** Jos WWW-asiakassovelluksen palvelun tila ei **ole Käynnissä**, kaksoisnapsauta palvelua, valitse **Käynnistä** ja valitse sitten **OK**. Ota palvelu tarvittaessa käyttöön valitsemalla **Käynnistystapa-ruudussa** **joko** Manuaalinen **tai** Automaattinen. 
    
> [!NOTE]
> Lisätietoja Resurssienhallinnassa avaamisen vianmäärityksestä on kohdassa [Avaa Resurssienhallinnassa.](https://go.microsoft.com/fwlink/?linkid=871665) Tutustu synkronointiin paremmana vaihtoehtona: [synkronoi SharePoint uuden OneDrive-synkronointisovellus kanssa.](https://go.microsoft.com/fwlink/?linkid=871666) 
  

