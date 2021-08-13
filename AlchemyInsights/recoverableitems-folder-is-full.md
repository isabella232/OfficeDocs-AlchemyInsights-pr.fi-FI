---
title: 1336 RecoverableItems-kansio on täynnä
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
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061753"
---
# <a name="the-recoverable-items-folder-is-full"></a>Palautettavat-kansio on täynnä

Jos Exchange Online, Palautettavat-kansion oletustallennustilaraja on 30 Gt. Palautettavat-kansion tallennustilaraja suurenee automaattisesti 100 Gigatavuun, jos postilaatikko asetetaan oikeusavustajapitoon, eDiscovery-pitoon tai jos se määritetään säilytyskäytännölle.

Kun Palautettavat-kansion tallennustilaraja on ylittyy, tämä vaikuttaa postilaatikon toimintoihin seuraavilla tavoilla:

- Käyttäjä ei voi poistaa kohteita postilaatikosta.

- Hallitun kansion avustaja ei voi poistaa kohteita säilytystunnisteen tai hallitun kansion asetusten perusteella.

- Postilaatikoissa, joissa on käytössä yhden kohteen palautus tai jotka on asetettu pitoon, kirjoitusta varten avatun sivun suojausprosessi ei voi säilyttää käyttäjän muokkaamista kohteista versioita.

- Jos postilaatikoiden valvontalokit ovat käytössä, mitään postilaatikon valvontalokimerkintöjä ei voi tallentaa Palautettavat-kansion Valvonta-alikansioon.

Jos postilaatikko ei ole pitossa, järjestelmänvalvojat voivat `Search-Mailbox -SearchDumpsterOnly -DeleteContent` poistaa kohteita Palautettavat-kansiosta Exchange Online PowerShellin komennolla. Lisätietoja on seuraavissa artikkeleissa:

- [Viestien etsiminen ja poistaminen](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Jos postilaatikot ovat pitoon, järjestelmänvalvojien on poistettava pito, ennen kuin he voivat poistaa kohteita Palautettavat-kansiosta. Lisätietoja on kohdassa [Pilvipohjaisten postilaatikoiden Palautettavat-kansion](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)kohteiden poistaminen .

Järjestelmänvalvojat voivat estää Palautettavat-kansion täydentymisen kasvattamalla pitoa olevien postilaatikoiden Palautettavat-kansion tallennustilarajaa ja määrittää postilaatikon säilytyskäytännön, joka siirtää kohteita Palautettavat-kansiosta käyttäjän arkistopostilaatikkoon. Katso [Pitoa olevien postilaatikoiden Palautettavat-kiintiön suurentaminen.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
