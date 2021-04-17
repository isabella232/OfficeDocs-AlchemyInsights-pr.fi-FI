---
title: Microsoft 365 -sovellusten asentaminen ei löytänyt Office-käyttöoikeuksiin liittyvää viestiä
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816485"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Microsoft 365 -sovellusten "Office-käyttöoikeuksia ei löytyi" -viestin asentaminen

Jos näyttöön tulee tämä sanoma, kokeile seuraavaa:

1. Tarkista palomuurin, virustentorjuntaohjelman ja välityspalvelimen asetukset ja varmista, että ne eivät estä Microsoft 365 -sovellusten Internet-yhteyttä. Katso [Microsoft 365:n URL-osoitteet ja IP-osoitealueet.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Poista ja [varaa uudelleen Office-käyttöoikeus käyttäjälle,](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) jota ongelma koskee. 
3. Avaa Office-sovellus ja [kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) olemassa olevista käyttäjätileistä.
4. Siirry kohtaan Windowsin asetukset >  >  **Sähköpostitilit & tilit** ja poista kaikki työtilit paitsi kyseinen tili.
5. Siirry kohtaan Windowsin asetukset >  >  **Tilit Käytä työtä tai koulua** ja katkaise kaikkien työtilien yhteys, paitsi kyseinen tili.
6. Palauta Officen aktivoinnin tila. [Ohjeet](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Kirjaudu sisään](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) käyttämällä käyttäjätiliä, jota ongelma koskee.

Katso lisää vianmääritysratkaisuja ohjeista [Ei käyttöomistajaa ja aktivointivirheitä Officessa.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)