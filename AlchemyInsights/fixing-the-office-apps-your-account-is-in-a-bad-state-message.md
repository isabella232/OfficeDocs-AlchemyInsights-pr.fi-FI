---
title: Sovellusten Microsoft 365-sovelluksen asentaminen Tilisi on virheellinen tila -viestissä
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
- "2558"
- "9000571"
ms.openlocfilehash: 68c4dfcc0500761f8ce5090fddb9f2ad58af77bc411c9e714b14c383fef177de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068233"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Korjaa Microsoft 365 "Tilisi on huonossa tilassa" -virhe

Voit korjata tämän virheen kokeilemalla seuraavia asetuksia tietokoneessa, johon ongelma vaikuttaa:

- Avaa Office-sovellus valitsemalla   >  **Tiedostotili**  >  **Kirjaudu ulos kaikista tileistä.** Kirjaudu uudelleen sisään käyttäjätilillä, jossa on kelvollinen käyttöoikeus. Saat lisätietoja ohjeartikkelista [Office-tilit](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Poista Office tunnistetiedot](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) tunnistetietojen Windows avulla.<br>
  **Huomautus:** Office 2016:n rekisteripolut ovat muuttuneet 16.0-arvoksi. Esimerkiksi \Software\Microsoft\Office\16.0\Common\Identity\
- Jos virhe ilmenee yhdistettäessä Office 365 Office 2013:n [avulla,](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) ota moderni todennus käyttöön Office asiakasohjelmassa.

Lisätietoja on kohdassa Muiden kuin selainsovellusten vianmääritys, jotka eivät voi kirjautua [Microsoft 365:ssä, Azuressa tai Intunessa.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)

