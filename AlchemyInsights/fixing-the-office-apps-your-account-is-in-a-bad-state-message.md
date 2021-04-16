---
title: Microsoft 365 -sovellusten asentaminen Tilisi on virheellinen tila -viestissä
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
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812533"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Microsoft 365 -sovellusten "Tilisi on huonossa tilassa" -virheen asentaminen

Voit korjata tämän virheen kokeilemalla seuraavia asetuksia tietokoneessa, johon ongelma vaikuttaa:

- Avaa Office-sovellus ja valitse  >  **Tiedostotili**  >  **Kirjaudu ulos kaikista tileistä.** Kirjaudu uudelleen sisään käyttämällä käyttäjätiliä, jolla on kelvollinen käyttöoikeus. Saat lisätietoja artikkelista [Office-tilit](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Poista Office-tunnistetiedot](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windowsin tunnistetietojen hallinnan avulla.<br>
  **Huomautus:** Office 2016:n rekisteripolut ovat muuttuneet 16.0-versioksi. Esimerkiksi \Software\Microsoft\Office\16.0\Common\Identity\
- Jos virhe ilmenee yhdistettäessä Office 365:een Office 2013:n [avulla,](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) ota moderni todennus käyttöön Office-asiakasohjelmassa.

Lisätietoja on kohdassa Muiden kuin selainsovellusten vianmääritys, jotka eivät voi kirjautua [Microsoft 365:ssä, Azuressa tai Intunessa.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)

