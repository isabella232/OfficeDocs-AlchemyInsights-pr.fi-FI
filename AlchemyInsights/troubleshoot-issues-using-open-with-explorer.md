---
title: Avaa Resurssienhallinnassa -sovelluksen ongelmien vianmääritys
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 0cbcfb506295d5732f7109be7a103bbdef530a529c7408c6d9d45a7b38a89915
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048153"
---
# <a name="fix-problems-with-open-with-explorer"></a>Avaa Resurssienhallinnassa -ongelmien ratkaiseminen

Avaa tiedostokirjasto -komennolla voit korjata yleisiä ongelmia SharePoint OneDrive Avaa **Resurssienhallinnassa -komennolla:** 
  
- Käytä Internet Explorer 10 Internet Explorer 11:tä. **Avaa Resurssienhallinnassa** -sovellus ei ole yhteensopiva muiden Microsoft Edge, Google Chromen, Firefoxin ja muiden kanssa. **Avaa Resurssienhallinnassa -kohta** ei ole käytettävissä kaikissa selaimissa Internet Exploreria lukuun ottamatta. 
    
- **Avaa Resurssienhallinnassa** -kohta ei ole käytettävissä kirjastojen modernissa SharePoint kanssa. Käytä **sen sijaan Näytä Resurssienhallinnassa -näkymää.** Valitse **Näytä asetukset** Näytä \> **Resurssienhallinnassa**. Resurssienhallinnassa näkymä ei ole yhteensopiva muiden Microsoft Edge, Google Chromen, Firefoxin ja muiden kanssa. **Näytä Resurssienhallinnassa vain** Internet Explorerissa. 
    
- Varmista, että WEBClient-palvelu on käynnissä. Kirjoita Windows-ruutuun suorita, valitse Suorita työpöytäsovellus, kirjoita services.msc ja paina Enter-näppäintä. Vieritä alaspäin WEBClient-palveluun ja varmista, että **Tila-sarakkeessa** näkyy "Käynnissä". Jos näin ei ole, kaksoisnapsauta palvelua, valitse **Käynnistä** ja valitse sitten **OK**. (Sinun on ehkä ensin otettava palvelu käyttöön valitsemalla **Käynnistystapa-ruudussa** **Joko** Manuaalinen **tai** Automaattinen.) 
    
> [!NOTE]
> Kirjaston avaaminen Resurssienhallinnassa on kätevää, jos haluat kopioida tai siirtää useita tiedostoja ja kansioita kerran, mutta jos haluat käyttää kirjastoa säännöllisesti, on suositeltavaa synkronoida se. Lisätietoja Resurssienhallinnassa avaamisen vianmäärityksestä on kohdassa [Avaa Resurssienhallinnassa.](https://go.microsoft.com/fwlink/?linkid=871665) Lisätietoja synkronoinnin määrittämisestä on kohdassa [tiedostojen SharePoint synkronointi uuden OneDrive-synkronointisovellus kanssa.](https://go.microsoft.com/fwlink/?linkid=871666)
  
Lisätietoja on artikkelissa Avaa Resurssienhallinnassa -komennon [käyttäminen SharePoint Onlinen](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) ongelmien vianmäärityksessä. 
  

