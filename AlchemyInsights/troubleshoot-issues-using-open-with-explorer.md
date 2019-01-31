---
title: Käyttämällä Avaa Explorerin ongelmien vianmääritys
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: c95f07b9fb7251442577c014e4005dbe3f92ceb4
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661748"
---
# <a name="fix-problems-with-open-with-explorer"></a>Avaa Explorer liittyvien ongelmien korjaaminen

Yleisten ongelmien avaamalla asiakirjakirjaston SharePoint- tai OneDrive **Avaa Explorerissa** -komennolla: 
  
- Käytä Internet Explorer 10 tai Internet Explorerin 11. **Avaa Explorerissa** ei ole yhteensopiva Microsoft Edge, Google Chrome, Firefox ja muut. **Avaa Explorerissa** ei ole käytettävissä kaikissa selaimissa kuin Internet Explorer. 
    
- **Avaa Explorerissa** ei ole käytettävissä SharePoint-kirjastoihin, Moderni kokemus. Käytä **Resurssienhallinta-näkymässä** . Valitse **Näytä asetukset** \> **Resurssienhallinta-näkymässä**. Resurssienhallinta-näkymässä ei ole yhteensopiva Microsoft Edge, Google Chrome, Firefox ja muut. **Resurssienhallinta-näkymässä** käytettävissä vain Internet Explorerissa. 
    
- Varmista, että WebClient-palvelu on käynnissä. Windows-hakuruutuun Suorita, tyyppi valitse Suorita desktop app, kirjoita services.msc ja paina sitten Enter. WebClient-palvelua kohtaan ja varmista, että **tila** -sarakkeessa näkyy ”käynnissä”. Jos näin ei ole, kaksoisnapsauta palvelua, napsauttamalla **Käynnistä-painiketta**ja valitse sitten **OK**. (Saatat joutua ensin otettava palvelu käyttöön valitsemalla **manuaalisen** tai **automaattisen** **käynnistyksen tyyppi** -ruudusta.) 
    
> [!NOTE]
> Kirjaston avaaminen Resurssienhallinta on kätevä, jos haluat kopioida tai siirtää useita tiedostoja ja kansioita, kun, mutta jos haluat käyttää säännöllisesti kirjastossa, suosittelemme synkronoit sen. Avattaessa tiedostoa Explorer-ongelmien vianmäärityksen, on [avoinna Resurssienhallinnassa](https://go.microsoft.com/fwlink/?linkid=871665). Katso tiedot synkronoinnin määrittäminen [OneDrive synkronointi uuden asiakkaan kanssa synkronointi SharePoint-tiedostot](https://go.microsoft.com/fwlink/?linkid=871666).
  
On lisätietoja artikkelissa [SharePoint Online-ongelmien vianmääritys ”Open kanssa Explorer”-komennon käyttämisestä](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) . 
  

