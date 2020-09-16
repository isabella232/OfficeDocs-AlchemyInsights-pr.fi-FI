---
title: Exchange-hallinta keskuksen säilytys käytännöt eivät toimi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740507"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Exchange-hallinta keskuksen säilytys käytännöt

Jos haluat, että suoritat automaattiset tarkistukset alla mainittuihin asetuksiin, valitse Edellinen-painike <--tämän sivun yläosassa ja kirjoita sitten sen käyttäjän Sähkö posti osoite, jolla on ongelmia säilytys käytäntöjen kanssa.

 **Ongelma:** Exchange-hallinta keskuksen uudet tai päivitetyt säilytys käytännöt eivät koske posti laatikoita tai kohteita ei siirretä Arkisto posti laatikkoon tai niitä ei poisteta. 
  
 **Perimmäiset syyt:**
  
- Tämä voi johtua siitä, että **Hallittujen kansioiden hallinta** ei ole käsitellyt käyttäjän posti laatikkoa. Hallittujen kansioiden avustaja yrittää käsitellä jokaista pilvipohjaisen organisaatiosi posti laatikkoa kerran seitsemän päivän välein. Jos muutat säilytys tunnisteen tai käytät eri säilytys käytäntöä posti laatikolle, voit odottaa, että hallittujen kansioiden avustaja käsittelee posti laatikkoa, tai voit käynnistää hallitun kansion avustajan käsittelemään tietyn posti laatikon suorittamalla Käynnistä-Managedfoldannestention-cmdlet-toiminnon. Tämän cmdlet-toiminnon suorittaminen on hyödyllistä säilytys käytännön tai säilytyksen tunniste asetusten testaamiseen tai vian määritykseen. Lisä tietoja on Ohje aiheessa [hallitun kansion avustajan suorittaminen](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Ratkaisu:** Käynnistä hallitun kansion avustaja tietylle posti laatikolle suorittamalla seuraava komento:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Tämä voi ilmetä myös, jos **RetentionHold** on **otettu käyttöön** posti laatikossa. Jos posti laatikko on asetettu RetentionHold-kohtaan, posti laatikon säilytys käytäntöä ei prosessoida tuona aikana. Lisä tietoja on kohdassa RetentionHold-asetus Katso: [Posti laatikon säilytyksen pito](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Ratkaisu**
    
  - Tarkasta RetentionHold-asetuksen tila tietyssä posti laatikossa [EXO PowerShellin](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)avulla:
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Suorita seuraava komento, jos haluat poistaa RetentionHold-toiminnon **käytöstä** tietyssä posti laatikossa:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Suorita sitten hallitun kansion avustaja uudelleen:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Huomautus:** Jos posti laatikko on pienempi kuin 10 Mt, hallittujen kansioiden hallinta ohjelma ei käsittele posti laatikkoa automaattisesti.
 
Lisä tietoja Exchange-hallinta keskuksen säilytys käytännöistä on kohdassa:
- [Säilytys Tunnisteet ja säilytys käytännöt](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Säilytys käytännön käyttäminen posti laatikoissa](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Säilytys tunnisteiden lisääminen tai poistaminen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Posti laatikkoon sijoitetun pidon tyypin selvittäminen](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
