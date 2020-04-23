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
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720249"
---
# <a name="the-recoverable-items-folder-is-full"></a>Palautettavat-kansio on täynnä

Exchange Online -postilaatikoissa Palautettavat kohteet -kansion oletustallennusrajoitus on 30 Gigatavua. Palautettavat-kansion tallennusraja nostetaan automaattisesti 100 Gigatavuun, jos postilaatikko asetetaan Oikeustoimiin liittyvään pitoon, eDiscovery-pitoon tai säilytyskäytäntöön.

Kun Palautettavat-kansio saavuttaa tallennusrajoituksen, postilaatikkotoiminto vaikuttaa seuraaviin tapoihin:

- Käyttäjä ei voi poistaa postilaatikon kohteita.

- Hallitun kansion avustaja ei voi poistaa kohteita säilytystunnisteen tai hallitun kansion asetusten perusteella.

- Postilaatikoissa, joiden yksittäisen kohteen palautus on käytössä tai jotka on sijoitettu pitoon, kopioinnin sivun suojausprosessi ei voi ylläpitää käyttäjän muokkaamien kohteiden versioita.

- Postilaatikoissa, joissa postilaatikon valvontaloki on käytössä, ei voi tallentaa postilaatikon valvontalokin merkintöjä Palautettavat-kansion Valvonta-alikansioon.

Jos postilaatikot eivät ole pidossa, järjestelmänvalvojat voivat poistaa palautettavat kohteet -kansion kohteiden poistamisesta Exchange Online PowerShellin `Search-Mailbox -SearchDumpsterOnly -DeleteContent` komennolla. Lisätietoja on seuraavissa artikkeleissa:

- [Viestien etsiminen ja poistaminen](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Haku-postilaatikko](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Pidossa olevien postilaatikoiden järjestelmänvalvojien on poistettava pito, ennen kuin he voivat poistaa kohteita Palautettavat-kansiosta. Lisätietoja on [ohjeaiheessa Pilvipohjaisten postilaatikoiden Palautettavat-kansion kohteiden poistaminen pidossa](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Järjestelmänvalvojat voivat pidentää palautettavat kohteet -kansion täyttämistä lisäämättä pitopostilaatikoiden Palautettavat-kansion tallennusrajoitusta ja määrittää postilaatikon säilytyskäytännön, joka siirtää kohteet Palautettavat-kansiosta käyttäjän arkistopostilaatikkoon. Katso [Pitopostilaatikoiden Palautettavat-kiintiön suurentaminen](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
