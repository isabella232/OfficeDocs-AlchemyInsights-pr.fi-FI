---
title: Exchange-hallintakeskuksen säilytyskäytännöt eivät toimi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502604"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Säilytyskäytännöt Exchange-hallintakeskuksessa

 **Numero:** Exchange-hallintakeskuksen äskettäin luodut tai päivitetyt säilytyskäytännöt eivät koske postilaatikoita tai kohteita ei siirretä arkistopostilaatikkoon tai poisteta. 
  
 **Perussyitä:**
  
- Tämä voi johtua siitä, että **hallitun kansion avustaja** ei ole käsitellyt käyttäjän postilaatikkoa. Hallitun kansion hallinta yrittää käsitellä pilvipohjaisen organisaation jokaista postilaatikkoa seitsemän päivän välein. Jos muutat säilytystunnistetta tai käytät postilaatikkoon eri säilytyskäytäntöä, voit odottaa, kunnes hallittu kansioavustin käsittelee postilaatikon, tai voit käynnistää hallitun kansion hallinnan suorittamalla Start-ManagedFolderAssistant-cmdlet-otoksen ja käynnistää tietyn postilaatikon. Tämän cmdlet-esityksen suorittaminen on hyödyllistä säilytyskäytännön tai säilytystunnisteen asetusten testaamisessa tai vianmäärityksessä. Lisätietoja on [ohjeaiheessa Hallitun kansion hallinnan suorittaminen](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Ratkaisu:** Käynnistä tietyn postilaatikon hallitun kansion hallintaohjelma suorittamalla seuraava komento:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Näin voi käydä myös, jos **RetentionHold** on otettu **käyttöön** postilaatikossa. Jos postilaatikko on sijoitettu Säilytyspalvelun säilyttämiseen, postilaatikon säilytyskäytäntöä ei käsitellä kyseisenä aikana. Lisätietoja RetentionHold-asetuksesta on kohdassa [Postilaatikon säilytyspito](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Ratkaisu:**
    
  - Tarkista [exo powershellin](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)postilaatikon RetentionHold-asetuksen tila:
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Poista RetentionHold **käytöstä** tietyssä postilaatikossa suorittamalla seuraava komento:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Suorita nyt hallitun kansion hallintaohjelma uudelleen:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Huomautus:** Jos postilaatikon koko on alle 10 megatavua, hallitun kansion hallinta ei käsittele postilaatikkoa automaattisesti.
 
Lisätietoja Exchange-hallintakeskuksen säilytyskäytännöistä on seuraavissa ohjeissa:
- [Säilytystunnisteet ja säilytyskäytännöt](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Säilytyskäytännön käyttäminen postilaatikoissa](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Säilytystunnisteiden lisääminen tai poistaminen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Postilaatikkoon sijoitetun pitoon asetetun pidon tyypin tunnistaminen](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
