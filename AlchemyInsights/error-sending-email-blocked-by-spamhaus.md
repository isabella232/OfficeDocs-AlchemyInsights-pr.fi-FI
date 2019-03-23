---
title: Virhe esti SpamHaus sähköpostin lähettäminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 7d6ad2667613ae948a4abcefafe8d91cf89d2418
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/22/2019
ms.locfileid: "30761630"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Virhe lähetettäessä sähköpostia: asiakkaan isäntä esti Spamhaus avulla

IP-osoite, joka lähetetty viesti on torjuttujen luettelon omistaa [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Syistä Spamhaus estää tartunnan saaneen tilit ovat tartunnan koneet julkisen IP-osoitteen ja Internet-palveluntarjoajan (ISP) käytäntöjen jakaminen. Mahdolliset korjaukset ovat seuraavat:
  
- Estetty saapuvien viestien, jossa voit määrittää Lähdepalvelimen sähköposti Office 365: ssä sinun on syy ja poistaa lohkon Spamhaus WWW-sivustosta.
    
- Estetty saapuvien viestien, jossa lähde-IP-osoite kuuluu jollekin toiselle Office 365-osoitteen omistaja on poistettava esto Spamhaus WWW-sivustosta. Jos IP-osoite-käytännön Block luetteloon (jaossa PBL), omistaja voi eri staattisen IP-osoitteen tai poistaa osoitteen jaossa PBL.
    
- Office 365-toimialueen estettyjen lähtevien viestien kohdata tämän virheen, jos Sanomat reititetään 3 osapuolen palvelun kautta. WHOIS haku-työkalun avulla voit löytää estetty IP-osoite omistaja.
    

