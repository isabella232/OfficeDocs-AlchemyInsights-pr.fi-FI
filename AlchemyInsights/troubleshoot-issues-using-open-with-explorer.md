---
title: Open with Explorerin käyttöön liittyvien ongelmien vianmääritys
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759689"
---
# <a name="fix-problems-with-open-with-explorer"></a>Open with Explorerin ongelmien korjaaminen

SharePointin tai OneDriven tiedostokirjaston avaamiseen liittyvien yleisten ongelmien korjaaminen **Avaa Resurssienhallinnassa** -komennolla: 
  
- Käytä Internet Explorer 10:tä tai Internet Explorer 11:tä. **Open with Explorer** ei ole yhteensopiva Microsoft Edgen, Google Chromen, Firefoxin ja muiden kanssa. **Avaa Resurssienhallinnassa** on poistettu käytöstä kaikissa selaimissa Internet Exploreria lukuun ottamatta. 
    
- **Avaa Resurssienhallinnan avulla** ei ole käytettävissä SharePoint-kirjastojen modernissa käyttökokemuksessa. Käytä sen sijaan **Resurssienhallinnassa näkymää.** Valitse **Resurssienhallinnassa Näytä asetukset** \> **.** Resurssienhallinnan näkymä ei ole yhteensopiva Microsoft Edgen, Google Chromen, Firefoxin ja muiden kanssa. **Näytä Resurssienhallinnassa,** joka on käytettävissä vain Internet Explorerissa. 
    
- Varmista, että WebClient-palvelu on käynnissä. Kirjoita Windowsin hakuruutuun suorita, valitse Suorita työpöytäsovellus, kirjoita services.msc ja paina sitten Enter-näppäintä. Vieritä alas WebClient-palveluun ja varmista, että **Tila-sarakkeessa** näkyy "Käynnissä". Jos näin ei ole, kaksoisnapsauta palvelua, napsauta **Käynnistä -painiketta**ja valitse sitten **OK**. (Sinun on ehkä ensin otettava palvelu käyttöön valitsemalla **Käynnistystapa-ruudusta** **Joko Manuaalinen** tai **Automaattinen.)** 
    
> [!NOTE]
> Kirjaston avaaminen Resurssienhallinnassa on kätevää, jos haluat kopioida tai siirtää useita tiedostoja ja kansioita kerran, mutta jos haluat työskennellä säännöllisesti kirjastossa, suosittelemme sen synkronointia. Lisätietoja Resurssienhallinnan avaamiseen liittyvien ongelmien vianmäärityksestä on [ohjeaiheessa AvaaMinen Resurssienhallinnassa](https://go.microsoft.com/fwlink/?linkid=871665). Lisätietoja synkronoinnin määrittämisestä on ohjeaiheessa [SharePoint-tiedostojen synkronoiminen uuden OneDrive-synkronointiohjelman kanssa](https://go.microsoft.com/fwlink/?linkid=871666).
  
Lisätietoja on artikkelissa [SharePoint Onlinen ongelmien vianmääritys Avaa Resurssienhallinnassa -komennon avulla.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) 
  

