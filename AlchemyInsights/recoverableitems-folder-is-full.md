---
title: 1336 RecoverableItems-kansio on täynnä
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510749"
---
# <a name="the-recoverable-items-folder-is-full"></a>Palautettavat-kansio on täynnä

Exchange Online -postilaatikoissa Palautettavat-kansion oletustallennusrajoitus on 30 Gigatavua. Palautettavat-kansion tallennusrajoitus nostetaan automaattisesti 100 gigatavuun, jos postilaatikko sijoitetaan oikeustoimiin pitoon, eDiscovery Holdiin tai säilytyskäytäntöön.

Kun Palautettavat-kansio saavuttaa tallennusrajan, tämä vaikuttaa postilaatikkotoimintoon seuraavilla tavoilla:

- Käyttäjä ei voi poistaa kohteita postilaatikosta.

- Hallitun kansion hallinta ei voi poistaa kohteita säilytystunnisteen tai hallittujen kansioiden asetusten perusteella.

- Postilaatikoissa, joiden yksittäinen kohde on otettu käyttöön tai jotka on sijoitettu pitoon, kopio-on-kirjoitussivun suojausprosessi ei voi ylläpitää käyttäjän muokkaamien kohteiden versioita.

- Postilaatikoissa, joissa postilaatikon valvontaloki on käytössä, postilaatikon valvontalokimerkintöjä ei voi tallentaa Palautettavat-kansion Valvonta-alikansioon.

Jos postilaatikossa ei ole pidossa, järjestelmänvalvojat voivat `Search-Mailbox -SearchDumpsterOnly -DeleteContent` poistaa Palautettavat-kansion kohteita Exchange Online PowerShellin komennolla. Lisätietoja on seuraavissa artikkeleissa:

- [Viestien etsiminen ja poistaminen](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Haku-postilaatikko](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Pidossa olevissa postilaatikoissa järjestelmänvalvojien on poistettava pito, ennen kuin he voivat poistaa kohteita Palautettavat-kansiosta. Lisätietoja on [ohjeaiheessa Pidossa olevien pilvipohjaisten postilaatikoiden Palautettavat-kansion kohteiden poistaminen](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Järjestelmänvalvojat voivat lisätä pidossa olevien postilaatikoiden Palautettavat-kansion tallennusrajoitusta ja määrittää postilaatikon säilytyskäytännön, joka siirtää kohteet Palautettavat-kansiosta käyttäjän arkistopostilaatikkoon. Lisätietoja [on ohjeaiheessa Pidossa olevien postilaatikoiden palautettavan sisällön kiintiön suurentaminen](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
