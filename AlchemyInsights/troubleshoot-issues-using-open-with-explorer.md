---
title: Avaa Resurssienhallinnassa-toiminnolla-ongelmien vian määritys
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742730"
---
# <a name="fix-problems-with-open-with-explorer"></a>Avaa Resurssienhallinnan ongelmien korjaaminen

Korjaa yleisiä ongelmia asiakirja kirjaston avaamisessa SharePointissa tai OneDrivessa **Avaa Resurssienhallinnassa-** komennolla: 
  
- Käytä Internet Explorer 10: tä tai Internet Explorer 11: tä. **Avaa Explorerilla** ei ole yhteensopiva Microsoft Edgen, Google Chromen, Firefoxin ja muiden kanssa. **Avaa Resurssienhallinnassa** ei ole käytössä kaikissa selaimissa, paitsi Internet Explorerissa. 
    
- **Avaa Resurssienhallinnassa** ei ole käytettävissä modernissa SharePoint-kirjastojen käyttö kokemessa. Käytä sen sijaan **näkymää Resurssienhallinnassa** . Valitse Resurssienhallinnan **Näytä asetukset** \> **-näkymä**. View in File Explorer ei ole yhteensopiva Microsoft Edge, Google Chrome, Firefox ja muut. **View in File Explorer** käytettävissä vain Internet Explorerissa. 
    
- Varmista, että WebClient-palvelu on käynnissä. Kirjoita Windows Search-ruutuun Suorita, valitse Suorita Työpöytä sovellus, kirjoita Services. msc ja paina sitten ENTER-näppäintä. Vieritä alaspäin WebClient-palveluun ja varmista, että **tila** sarakkeessa näkyy "Running". Jos se ei ole, kaksoisnapsauta palvelua, valitse **Käynnistä**ja valitse sitten **OK**. (Sinun on ehkä ensin otettava palvelu käyttöön valitsemalla **Käynnistys tyyppi** -ruudusta joko **Manuaalinen** tai **Automaattinen** .) 
    
> [!NOTE]
> Kirjaston avaaminen Resurssienhallinnassa on kätevää, jos sinun on kopioitava tai siirrettävä useita tiedostoja ja kansioita kerran, mutta jos haluat työskennellä säännöllisesti kirjastossa, suosittelemme sen synkronoimista. Jos haluat suorittaa Resurssienhallinnan ongelmien vian määrityksen, katso [Avaa Resurssienhallinnassa](https://go.microsoft.com/fwlink/?linkid=871665). Lisä tietoja synkronoinnin määrittämisestä [on artikkelissa SharePoint-tiedostojen synkronointi uuden OneDrive-synkronointi asiakkaan kanssa](https://go.microsoft.com/fwlink/?linkid=871666).
  
Katso lisä tietoja artikkelista [kuinka käyttää avaa Exploreria-komentoa SharePoint Onlinen ongelmien vian määritykseen](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) . 
  

