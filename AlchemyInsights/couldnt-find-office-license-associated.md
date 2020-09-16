---
title: Fixing Microsoft 365-sovellukset eivät löytäneet Office-käyttö oikeuksiin liittyvää viestiä
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747692"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Microsoft 365-sovellusten korjaaminen "Office-käyttö oikeuksien etsimistä ei löytynyt"-viesti

Jos saat tämän viestin, kokeile seuraavaa:

1. Tarkista palo muurin, virustentorjuntaohjelman ja välitys palvelimen asetukset ja varmista, että ne eivät estä Internet-yhteyttä Microsoft 365-sovelluksiin. Katso [Microsoft 365-URL-osoitteet ja IP-osoite alueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Poista kyseisen käyttäjän [Office-käyttö oikeus ja määritä se](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) uudelleen. 
3. Avaa Office-sovellus ja [Kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) olemassa olevista käyttäjä tileistäsi.
4. Siirry kohtaan Windowsin asetukset > **tilit**  >  -**Sähkö posti & tilit**ja poista kaikki työtilit, paitsi kyseinen tili.
5. Siirry kohtaan Windowsin asetukset > **tilit**  >  **käyttää työpaikan tai oppi laitoksen**ja Katkaise kaikki työtilit, paitsi kyseinen tili.
6. Palauta Officen aktivoinnin tila. [Ohjeet](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Kirjaudu sisään](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) haavoittuvuuden sisältävän käyttäjä tilin avulla.

Lisä tietoja vian määrityksestä on kohdassa käyttö oikeuden sisältävän [tuotteen ja aktivointi virheen määrittäminen Officessa](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).