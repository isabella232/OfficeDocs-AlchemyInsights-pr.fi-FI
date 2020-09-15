---
title: Ongelmia, jotka liittyvät Microsoft 365-sovelluksiin kirjautumiseen
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
- "9000571"
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695320"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Microsoft 365-sovellusten korjaaminen "Valitettavasti toinen organisaatiosi tili on jo allekirjoitettu" viesti

Voit korjata ongelman toimimalla seuraavasti:

- Poista kaikki työtilit, paitsi heikkouden sisältävä tili, käyttämällä Windowsin asetuksia > **käyttää työpaikan tai oppi laitoksen**tietoja.
- [Poista Officen tunniste tiedot käyttämällä Windows Credential](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Manageria.<br/>
    **Huomautus:** Office 2016-rekisteri polut ovat muuttuneet 16,0-asetuksiksi. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Avaa Office-sovellus ja valitse **tiedosto**  >  **tili**  >  **Kirjaudu ulos**. Kirjaudu sitten sisään käyttämällä käyttäjä tiliä, jolla on voimassa oleva käyttö oikeus. Saat lisätietoja artikkelista [Office-tilit](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Jos sinulla on Mac-kone, lue kohta [Kirjautuminen Office 2016 for Mac -sovellukseen ei onnistu](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Lisä tietoja [on kohdassa "Valitettavasti toinen organisaatiosi tili on jo kirjautuneena tähän tieto koneeseen" Officessa](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).