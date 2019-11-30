---
title: Office-sovellusten korjaaminen ei löytänyt Office-lisenssien liitettyä viestiä
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1820cdb83a1adf36b4e7d0898ecdf8097eb6f0f3
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627915"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a>Office-sovellusten korjaaminen ei löytänyt Office-lisenssejä liitetty-sanoma

Jos tämä sanoma tulee näyttöön, kokeile seuraavia:

1. Tarkista palo muuri-, virustentorjuntaohjelmisto-ja välitys palvelin asetukset ja varmista, etteivät ne estä Internet-pääsyä Office-sovelluksiin. Katso [Office 365-URL-osoitteet ja IP-osoite alueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Poista haavoittuvuuden sisältävän käyttäjän [Office-käyttö oikeus ja määritä se uudelleen](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) . 
3. Avaa Office-sovellus ja [Kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) aiemmin luodusta käyttäjä tileistä.
4. Siirry Windows-asetuksiin > **tilit** > **Sähkö posti & tilit**ja poista kaikki työtilit paitsi haavoittuvuuden sisältävän tilin.
5. Siirry Windows-asetuksiin > **tilien** > **käyttö oikeus työ tai koulu**ja Katkaise kaikki työtilit lukuun ottamatta tiliä, jota haavoittuvuus koskee.
6. Palauta Officen aktivointi tila. [Ohjeet](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Kirjaudu sisään](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) haavoittuvuuden sisältävän käyttäjä tilin avulla.

Lisä vian määritys ratkaisuja on kohdassa [Officen käyttö oikeuden ja aktivointi virheiden poistaminen](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).