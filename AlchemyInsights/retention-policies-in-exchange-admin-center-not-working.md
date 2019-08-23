---
title: Säilytyskäytännöt Keskikaiuttimen Admin ei toimi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 5d7b62546397c13b37540e8797b31123b2880280
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551340"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Säilytyskäytännöt-Exchange-hallintakeskukseen

 **Ongelma:** Äskettäin luotu tai päivitetty Exchange Admin Centerissä säilytyskäytännöt soveltavat ei postilaatikoihin tai kohteita ei Arkistoi postilaatikko siirretään tai poistetaan. 
  
 **Pääsyyt:**
  
- Tämä voi johtua siitä että **Hallitun kansion avustajan** ei käsitelty käyttäjän postilaatikkoon. Hallitun kansion avustajan yrittää käsitellä jokaisen postilaatikon pilvipohjainen organisaatiosi seitsemän päivän välein. Jos muutat pidätys tunnisteen tai soveltaa eri säilytyskäytäntö postilaatikkoon, voit odottaa, kunnes hallitun kansion avustaa käsittelee postilaatikon, tai voit suorittaa Start-ManagedFolderAssistant-cmdlet-komento Käynnistä-hallitun kansion avustajan käsittelemään tiettyä postilaatikko. Käytössä tämä cmdlet-komento on hyödyllinen testaamisessa ja vianmäärityksessä tai säilytyskäytäntö säilytysasetukset tunniste. Saat lisätietoja seuraavasta [suorittaa hallitun kansion avustajan](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Ratkaisu:** Suorita seuraava komento käynnistää-hallitun kansion avustajan tietylle postilaatikolle:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Tämä saattaa myös ilmetä, jos **RetentionHold** on **otettu** käyttöön postilaatikon. Jos RetentionHold sijoitettu postilaatikko, säilytyskäytäntö-postilaatikko ei käsitellä samaan aikaan. Saat enemmän informaton-RetentionHold asetus Katso: [Postilaatikon pidätys pidä](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Ratkaisu:**
    
  - Tietyn postilaatikon [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)-RetentionHold-asetuksen tarkistaminen:
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Suorita seuraava komento **poistaa** RetentionHold tietyn postilaatikon:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Nyt uudelleen suorittaa hallitun kansion avustajan:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Huomautus:** Jos postilaatikko on alle 10 Mt, hallitun kansion avustajan ei automaattisesti käsittelee postilaatikon.
 
Saat lisätietoja Exchange-Admin Centerissä säilytyskäytännöt:
- [Pidätys tunnisteet ja säilytyskäytäntöjä](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Käytä säilytyskäytäntöä postilaatikot](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Lisää tai poistaa tunnisteet pidätys](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Miten tunnistaa pidon tyyppi sijoitettu postilaatikkoon](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
