---
title: Tilin virheellisen tila viestin korjaaminen Microsoft 365-sovelluksissa
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744542"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Microsoft 365-sovellusten korjaaminen "tilisi on väärässä tilassa"-virhe

Voit korjata tämän virheen kokeilemalla seuraavia vaihto ehtoja haavoittuvuuden sisältävään tieto koneeseen:

- Avaa Office-sovellus ja valitse **tiedosto**  >  **tili**  >  **Kirjaudu ulos kaikista tileistäsi**. Kirjaudu uudelleen sisään käyttämällä käyttäjä tiliä, jolla on voimassa oleva käyttö oikeus. Saat lisätietoja artikkelista [Office-tilit](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Poista Officen tunniste tiedot käyttämällä Windows Credential](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Manageria.<br>
  **Huomautus:** Office 2016-rekisteri polut ovat muuttuneet 16,0-asetuksiksi. Esimerkiksi \Software\microsoft\office\16.0\common\identifi-\
- Jos virhe ilmenee, kun muodostat yhteyden Office 365-palveluun Office 2013-sovelluksen avulla, ota käyttöön Office-asiakas ohjelman [moderni todentaminen](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) .

Lisä tietoja on Ohje aiheessa [muiden kuin selain sovellusten, jotka eivät voi kirja utua Microsoft 365-, Azure-tai Intune-sovellukseen, vian määritys](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

