---
title: Office Microsoft 365 sovellusten asentaminen ei löytänyt Office-käyttöoikeuksiin liittyvää viestiä
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
ms.openlocfilehash: a65610dc5f88eeb4195e48131f08940758d0dfac0710502e0e15ab5f661c5719
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069601"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Office-Microsoft 365 liittyvien sovellusten asentaminen ei löytänyt liitettyä Office-käyttöoikeutta -viesti

Jos näyttöön tulee tämä sanoma, kokeile seuraavaa:

1. Tarkista palomuurin, virustentorjuntaohjelman ja välityspalvelimen asetukset ja varmista, että ne eivät estä Microsoft 365 internet-yhteyttä. Katso [Microsoft 365 URL-osoitteita ja IP-osoitealueita.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Poista [ja Office käyttäjän](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) käyttöoikeus uudelleen. 
3. Avaa Office-sovellus ja [kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) olemassa olevista käyttäjätileistä.
4. Siirry Windows Asetukset > **sähköpostitilit**  >  **& tilit** ja poista kaikki työtilit paitsi kyseinen tili.
5. Siirry Windows Asetukset > **tilit**  >  **Käytä työtä tai koulua** ja katkaise kaikkien työtilien yhteys lukuun ottamatta tiliä, johon ongelma vaikuttaa.
6. Palauta Officen aktivoinnin tila. [Ohjeet](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Kirjaudu sisään](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) käyttämällä käyttäjätiliä, jota ongelma koskee.

Katso muita vianmääritysratkaisuja ohjeista [Ei käyttöomistajaa ja aktivointivirheitä Office.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)