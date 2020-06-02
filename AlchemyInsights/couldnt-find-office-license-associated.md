---
title: Office-sovellusten korjaaminen Office-käyttöoikeuteen liittyvää viestiä ei löytynyt
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
ms.openlocfilehash: 887be4bee2bd1562bdc3b29783e9deafe47d8d57
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505864"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a>Office-sovellusten "Office-käyttöoikeuksia ei löytynyt" -sanoman korjaaminen

Jos näyttöön tulee tämä sanoma, kokeile seuraavaa:

1. Tarkista palomuurin, virustentorjuntaohjelmiston ja välityspalvelimen asetukset ja varmista, että ne eivät estä Office-sovellusten Internet-käyttöä. Lisätietoja on [microsoft 365:n URL-osoitteissa ja IP-osoitealueissa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Poista [Office-käyttöoikeus](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ja määritä se uudelleen haavoittuvuuden sisältävälle käyttäjälle. 
3. Avaa Office-sovellus ja [kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) olemassa olevista käyttäjätileistä.
4. Siirry Windowsin asetukset > **Tilit**  >  **Sähköposti & -tileille**ja poista kaikki työtilit kyseistä tiliä lukuun ottamatta.
5. Siirry Windowsin asetukset > **Tilit**  >  **Accessin työpaikan tai oppilaitoksen**käyttöön ja katkaise kaikkien työtilien yhteys lukuun ottamatta tiliä, jota haavoittuvuus koskee.
6. Palauta Officen aktivoinnin tila. [Ohjeet](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Kirjaudu sisään](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) käyttämällä kyseistä käyttäjätiliä.

Lisätietoja vianmäärityksestä on artikkelissa [Käyttöoikeudeton tuote- ja aktivointivirheet Officessa](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).