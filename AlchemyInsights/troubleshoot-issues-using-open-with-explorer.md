---
title: Avaa Resurssienhallinnassa-toiminnon ongelmien vian määritys
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
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659055"
---
# <a name="fix-problems-with-open-with-explorer"></a>Avaa Resurssienhallinnassa-ongelmien korjaaminen

Yleisten ongelmien korjaaminen avaamalla tiedosto Kirjasto SharePointissa tai OneDrivessa **Avaa Resurssienhallinnassa-** komennon avulla: 
  
- Käytä Internet Explorer 10: tä tai Internet Explorer 11-ohjelmistoa. **Avaa Resurssienhallinnassa** ei ole yhteensopiva Microsoft Edgessä, Google Chromessa, Firefoxissa ja muissa. **Avaa Resurssienhallinnassa** ei ole käytössä kaikissa selaimissa paitsi Internet Explorerissa. 
    
- **Avaa Resurssienhallinnassa-** toiminto ei ole käytettävissä SharePoint-kirjastojen nykyaikaisessa käyttö kokemuksessa. Käytä **Näytä Resurssienhallinnassa-** komentoa. Valitse **Näytä asetukset** \> **-näkymä Resurssienhallinnassa**. Näytä Resurssienhallinnassa ei ole yhteensopiva Microsoft Edgessä, Google Chromessa, Firefoxissa ja muissa. **Näytä Resurssienhallinnassa** -kohdassa käytettävissä vain Internet Explorerissa. 
    
- Varmista, että WebClient-palvelu on käynnissä. Kirjoita Windowsin haku ruutuun Suorita, valitse Suorita Työpöytä sovellus, kirjoita Services. msc ja paina sitten ENTER-näppäintä. Vieritä alas WebClient-palveluun ja varmista, että **tila** -sarakkeessa lukee "Running". Jos se ei onnistu, kaksoisnapsauta palvelua, valitse **Käynnistä**ja valitse sitten **OK**. (Sinun on ehkä ensin otettava palvelu käyttöön valitsemalla **Käynnistys tapa** -ruudussa joko **Manuaalinen** tai **Automaattinen** .) 
    
> [!NOTE]
> Kirjaston avaaminen Resurssienhallinnassa on kätevää, jos sinun täytyy kopioida tai siirtää useita tiedostoja ja kansioita kerran, mutta jos haluat työskennellä kirjastossa säännöllisesti, suosittelemme sen synkronointia. Lisä tietoja Resurssienhallinnan avaamis ongelmien vian määrityksestä on kohdassa [Avaa Resurssienhallinnassa](https://go.microsoft.com/fwlink/?linkid=871665). Lisä tietoja synkronoinnin määrittämisestä on Ohje aiheessa [SharePoint-tiedostojen synkronointi uuden OneDrive-synkronointi sovelluksen avulla](https://go.microsoft.com/fwlink/?linkid=871666).
  
Katso lisä tietoja artikkelista [Avaa Resurssienhallinnassa-komennon käyttäminen SharePoint Onlinen ongelmien vian määrityksessä](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) . 
  

