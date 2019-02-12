---
title: Siirtää sähköpostiviestejä postilaatikon arkisto
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a631af20e28a531a40f078e290239a372c38ab74
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29941703"
---
Ongelmia arkistoon postilaatikon kohteiden arkistoimisen. Varmista, että olet tehnyt seuraavat toimet:
  
1. Vahvista, että **Arkistoi postilaatikko** on käytössä. Jos et arkistoi postilaatikko käyttöön [tämän artikkelin](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) ohjeiden avulla. 
    
2. Valitse Exchange-hallintakeskukseen **Pidätys tunnisteet** **Yhteensopivuuden**hallinta, **pidätys tunnisteen** luominen-toiminnolla **siirtää arkisto** sisältää halutun **Pidätys ikä**.
    
3. -Admin Keskikaiuttimen **Säilytyskäytännöt**, **Säilytyskäytännön** luominen ja **siirtää arkiston** säilytyksen tunnisteen lisääminen politiikan. 
    
4. [Säilytyskäytännön määrittäminen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) tietyn käyttäjän postilaatikkoon. Samaa käytäntöä sovelletaan sekä **ensisijaisen** että **Arkistoi** postilaatikko. 
    
Käyttäjän postilaatikkoon on nyt siirtää kohteita Arkistoi postilaatikko arkisto-käytäntöä. Saatat joutua pakottamaan hallitun kansion avustajan (MFA) ja uusien asetusten käyttäminen käyttäjän postilaatikkoon. Suorittamalla seuraavan komennon käynnistäminen-hallitun kansion avustajan tietyn postilaatikon samalla [yhdistetty EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) : 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Lisätietoja arkisto-käytännön määrittämisestä on ohjeaiheessa [arkistoinnin ja poistamisen käytännön postilaatikoita varten määritetty](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

