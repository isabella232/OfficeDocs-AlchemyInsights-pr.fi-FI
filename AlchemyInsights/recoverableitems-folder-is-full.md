---
title: 1336 Recovertableitems-kansio on täynnä
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
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741264"
---
# <a name="the-recoverable-items-folder-is-full"></a>Palautettavat-kansio on täynnä

Exchange Online-posti laatikot: Palautettavat-kansion oletus tallennus tilan enimmäismäärä on 30 Giga tavua. Palautettavat-kansion tallennus tilan enimmäismäärä kasvaa automaattisesti 100 Giga tavuun, jos posti laatikko on asetettu oikeus toimiin liittyvään pitoon, eDiscoveryn pitoon tai kun se on määritetty säilytys käytännölle.

Kun Palautettavat-kansion tallennus tila on ylittyä, posti laatikko toimintoon vaikuttavat seuraavat asiat:

- Käyttäjä ei voi poistaa kohteita posti laatikosta.

- Hallitun kansion avustaja ei voi poistaa kohteita säilytys tunnisteen tai hallittujen kansioiden asetusten perusteella.

- Jos posti laatikoissa on otettu käyttöön yksi kohde tai ne on sijoitettu pitoon, kopio sivun suojaus prosessi ei voi ylläpitää käyttäjän muokkaamien kohteiden versioita.

- Posti laatikoiden valvonta lokin merkintöjä ei voi tallentaa Palautettavat-kansion tarkastukset-alikansioon, jos posti laatikon valvonta loki on käytössä.

Jos posti laatikot eivät ole pidossa, järjestelmänvalvojat voivat `Search-Mailbox -SearchDumpsterOnly -DeleteContent` poistaa kohteita palautettavat-kansiosta käyttämällä Exchange Online PowerShellin komentoa. Lisätietoja on seuraavissa artikkeleissa:

- [Viestien etsiminen ja poistaminen](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Haku-posti laatikko](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Jos käytössä on pidossa olevat posti laatikot, järjestelmänvalvojien on poistettava pito, ennen kuin he voivat poistaa kohteita palautettavat-kansiosta. Lisä tietoja on Ohje aiheessa [pidossa olevien pilvipohjaisten posti laatikoiden Palautettavat-kansion kohteiden poistaminen](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Jos haluat estää Palautettavat-kansion täysimääräisen tulemisen, järjestelmänvalvojat voivat suurentaa pidossa olevien posti laatikoiden Palautettavat-kansion tallennus tilan rajoitusta ja määrittää posti laatikon säilytys käytännön, joka siirtää kohteita palautettavat-kansiosta käyttäjän Arkisto posti laatikkoon. Katso lisä tietoja [pidossa olevien posti laatikoiden palautettavat-kiintiön korottamisesta](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
