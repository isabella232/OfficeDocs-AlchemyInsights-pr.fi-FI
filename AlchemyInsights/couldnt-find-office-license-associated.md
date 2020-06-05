---
title: Microsoft 365 -sovellusten korjaaminen Office-käyttöoikeuksille ei löytynyt viestiä
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
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580438"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Microsoft 365 -sovellusten "Office-käyttöoikeuksia ei löytynyt" -sanoman korjaaminen

Jos näyttöön tulee tämä sanoma, kokeile seuraavaa:

1. Tarkista palomuurin, virustentorjuntaohjelmiston ja välityspalvelimen asetukset ja varmista, että ne eivät estä Microsoft 365 -sovellusten Internet-käyttöä. Lisätietoja on [microsoft 365:n URL-osoitteissa ja IP-osoitealueissa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Poista [Office-käyttöoikeus](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ja määritä se uudelleen haavoittuvuuden sisältävälle käyttäjälle. 
3. Avaa Office-sovellus ja [kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) olemassa olevista käyttäjätileistä.
4. Siirry Windowsin asetukset > **Tilit**  >  **Sähköposti & -tileille**ja poista kaikki työtilit kyseistä tiliä lukuun ottamatta.
5. Siirry Windowsin asetukset > **Tilit**  >  **Accessin työpaikan tai oppilaitoksen**käyttöön ja katkaise kaikkien työtilien yhteys lukuun ottamatta tiliä, jota haavoittuvuus koskee.
6. Palauta Officen aktivoinnin tila. [Ohjeet](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Kirjaudu sisään](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) käyttämällä kyseistä käyttäjätiliä.

Lisätietoja vianmäärityksestä on artikkelissa [Käyttöoikeudeton tuote- ja aktivointivirheet Officessa](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).