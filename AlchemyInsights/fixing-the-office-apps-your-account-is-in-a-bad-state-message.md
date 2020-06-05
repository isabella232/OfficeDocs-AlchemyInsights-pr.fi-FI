---
title: Microsoft 365 -sovellusten korjaaminen Tilisi on huonossa tilassa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: 264307f23a349ef4ebf40f48ddbcddd3216a4927
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580114"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Microsoft 365 -sovellusten korjaaminen "Tilisi on huonossa kunnossa" -virhe

Voit korjata tämän virheen kokeilemalla seuraavia asetuksia haavoittuvuuden sisältävässä tietokoneessa:

- Avaa Office-sovellus **File**ja valitse  >  **Tiedostotili**  >  **Kirjaudu ulos kaikista tileistä**. Kirjaudu uudelleen sisään käyttäjätilillä, jolla on voimassa oleva käyttöoikeus. Saat lisätietoja artikkelista [Office-tilit](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Tyhjennä Officen tunnistetiedot](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windowsin tunnistetietojen hallinnan avulla.<br>
  **Huomautus:** Office 2016:n rekisteripolut ovat muuttuneet 16.0:ksi. Esimerkiksi \Software\Microsoft\Office\16.0\Common\Identity\
- Jos virhe ilmenee muodostettaessa yhteyttä Office 365:een Office 2013:n avulla, ota office-asiakasohjelman [nykyaikainen todennus käyttöön.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Lisätietoja on [ohjeaiheessa Muiden kuin selainsovellusten vianmääritys, jotka eivät pysty kirjautumaan Microsoft 365:ään, Azureen tai Intuneen](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

