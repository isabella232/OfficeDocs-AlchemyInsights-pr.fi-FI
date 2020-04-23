---
title: Exchange Admin Centerin säilytyskäytännöt eivät toimi
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
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742430"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Exchange Admin Centerin säilytyskäytännöt

 **Numero:** Exchange-hallintakeskuksen äskettäin luodut tai päivitetyt säilytyskäytännöt eivät koske postilaatikoita tai kohteita ei siirretä arkistopostilaatikkoon tai poisteta. 
  
 **Perussyitä:**
  
- Tämä voi johtua siitä, **että hallitun kansion avustaja** ei ole käsitellyt käyttäjän postilaatikkoa. Hallitun kansion avustaja yrittää käsitellä kaikki pilvipohjaisen organisaatiosi postilaatikot seitsemän päivän välein. Jos muutat säilytystunnistetta tai käytät eri säilytyskäytäntöä postilaatikossa, voit odottaa, kunnes hallitun kansion tuki käsittelee postilaatikon, tai voit käynnistää Hallitun kansion hallinnan suorittamalla Start-ManagedFolderAssistant-cmdlet-tiedoston ja käsitellä tietyn postilaatikon. Tämän cmdlet-tiedoston suorittaminen on hyödyllistä säilytyskäytännön tai säilytystunnisteasetusten testaamisessa tai vianmäärityksessä. Lisätietoja on [ohjeaiheessa Hallitun kansion hallinnan suorittaminen](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Ratkaisu:** Käynnistä tietyn postilaatikon hallitun kansion hallinta:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Tämä voi tapahtua myös, jos **RetentionHold** on otettu **käyttöön** postilaatikossa. Jos postilaatikko on sijoitettu RetentionHold-pitoon, postilaatikon säilytyskäytäntöä ei käsitellä kyseisenä aikana. Lisätietoja RetentionHold-asetuksesta on kohdassa [Postilaatikon säilytyspito .](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
    
    **Ratkaisu:**
    
  - Tarkista tietyn postilaatikon RetentionHold-asetuksen tila [EXO powershell -kohdassa:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Poista RetentionHold käytöstä tietyssä postilaatikossa **suorittamalla** seuraava komento:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Suorita hallitun kansion avustaja uudelleen:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Huomautus:** Jos postilaatikon koko on pienempi kuin 10 megatavua, hallitun kansion avustaja ei käsittele postilaatikkoa automaattisesti.
 
Lisätietoja Exchange-hallintakeskuksen säilytyskäytännöistä on seuraavissa ohjeissa:
- [Säilytystunnisteet ja säilytyskäytännöt](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Säilytyskäytännön käyttäminen postilaatikoissa](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Säilytystunnisteiden lisääminen tai poistaminen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Postilaatikkoon sijoitetun pidon tyypin tunnistaminen](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
