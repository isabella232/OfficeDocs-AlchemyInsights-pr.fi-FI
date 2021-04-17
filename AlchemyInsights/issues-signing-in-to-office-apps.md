---
title: Microsoft 365 -sovelluksiin kirjautumisongelmat
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
- "9000571"
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833072"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Microsoft 365 -sovellusten "Valitettavasti toinen organisaatiosi tili on jo kirjautunut sisään" -viesti

Voit korjata ongelman toimimalla seuraavasti:

- Poista kaikki työtilit lukuun ottamatta tilejä, joihin tämä vaikuttaa, käyttämällä Windows-> **käytä työtä tai koulua.**
- [Poista Office-tunnistetiedot](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windowsin tunnistetietojen hallinnan avulla.<br/>
    **Huomautus:** Office 2016:n rekisteripolut ovat muuttuneet 16.0-versioksi. (Esim: \Software\Microsoft\Office\16.0\Common\Identity\)
- Avaa Office-sovellus ja valitse  >  **Tiedostotili**  >  **Kirjaudu ulos**. Kirjaudu sitten sisään käyttämällä käyttäjätiliä, jolla on kelvollinen käyttöoikeus. Saat lisätietoja artikkelista [Office-tilit](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Jos sinulla on Mac-kone, lue kohta [Kirjautuminen Office 2016 for Mac -sovellukseen ei onnistu](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Lisätietoja on [Officen kohdassa "Organisaatiosi](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)toinen tili on jo kirjautuneena tähän tietokoneeseen".