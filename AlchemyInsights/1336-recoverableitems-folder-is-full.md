---
title: 1336 RecoverableItems kansio on täynnä
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: ee96abfa179c36ebaf43dbd327d4608b849395d3
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28286762"
---
# <a name="the-recoverable-items-folder-is-full"></a>Palautettavat kohteet-kansio on täynnä

Office 365-postilaatikot Exchange Online-palautettavat kohteet-kansio oletusarvoisesti enimmäiskoko on 30 GB. Palautettavat kohteet-kansion enimmäiskoko on automaattisesti kasvoi 100 GB Jos postilaatikko on sijoitettu pidä oikeudenkäyntiä eDiscovery pito tai Office 365-säilytyskäytäntö on määritetty.
  
Kun palautettavat kohteet-kansion enimmäiskoko, postilaatikko-toiminto vaikuttaa seuraavilla tavoilla:
  
- Käyttäjä voi poistaa postilaatikon kohteita.
    
- Hallitun kansion avustajan voi poistaa kohteita pidätys tunniste tai hallitun kansion asetusten perusteella.
    
- Postilaatikot, jotka ovat yksittäisen kohteen palauttaminen käytössä tai ovat pidossa, copy-kirjoittaa sivulla suojauksen prosessi ei voi ylläpitää käyttäjä ryhtyy muokkaamaan kohdeversioiden.
    
- Postilaatikot, joilla valvoa kirjaaminen on otettu käyttöön postilaatikon postilaatikko ei ole valvonnan tapahtumat voidaan tallentaa tarkastuksia palautettavat kohteet-kansion alikansioon.
    
Postilaatikot, jotka eivät ole estetty, järjestelmänvalvojat voivat käyttää `Search-Mailbox -SearchDumpsterOnly -DeleteContent` komento Exchange Online PowerShell poistaa kohteita palautettavat kohteet-kansiossa. Lisätietoja on seuraavissa ohjeaiheissa: 
  
- [Etsi ja poista viestejä](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [Search-Mailbox-](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
Pidossa olevat postilaatikot valvojat ovat pidosta, ennen kuin he voivat palauttaa kohteet-kansiosta poistettuja kohteita. Lisätietoja [kerrytettävissä olevan kansion pilvipohjainen postilaatikoita, pidä kohteet kohteiden poistaminen](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).
  
Voit estää tulemasta koko palautettavat kohteet-kansio, järjestelmänvalvojat lisäävät kerrytettävissä oleva nimikkeiden kansiota postilaatikoita varten hallussaan ja, jossa nimikkeitä siirretään palautettavat kohteet-kansioon arkistoon käyttäjän postilaatikon säilytyskäytäntö määritetty enimmäiskoko postilaatikko. Lisätietoja [kerrytettävissä kohteet kiintiön postilaatikoita, pidä kasvattaa](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
  

