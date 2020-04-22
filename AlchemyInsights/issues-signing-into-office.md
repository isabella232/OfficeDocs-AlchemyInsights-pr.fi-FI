---
title: Office-sovelluksiin kirjautumisongelmat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762993"
---
# <a name="issues-signing-in-to-office-apps"></a>Office-sovelluksiin kirjautumisongelmat

Voit korjata Office-sovellusten kirjautumisongelmat seuraavasti:

- Poista kaikki työtilit, paitsi kyseinen tili, käyttämällä Windowsin asetuksia > **Accessin työ- tai oppilaitokseen**.
- [Tyhjennä Office-tunnistetiedot](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windowsin tunnistetietojen hallinnan avulla.<br/>
    **Huomautus:** Office 2016:n rekisteripolut ovat muuttuneet muotoon 16.0. (Esim: \Software\Microsoft\Office\16.0\Common\Identity\)
- Avaa Office-sovellus ja valitse > **Tiedostotili** > **Kirjaudu ulos**. **File** Kirjaudu sitten sisään käyttäjätilillä, jolla on voimassa oleva käyttöoikeus. Saat lisätietoja artikkelista [Office-tilit](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Jos sinulla on Mac-kone, lue kohta [Kirjautuminen Office 2016 for Mac -sovellukseen ei onnistu](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Jos virheet tapahtuvat muodostettaessa yhteyttä Microsoft 365:een Office 2013:n avulla, ota office-asiakasohjelman moderni todennus käyttöön.

Lisätietoja on seuraavissa artikkeleissa:
- [Kirjautuminen Microsoft 365:een, Azureen tai Intuneen ei onnistu](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Yhteysongelmat kirjautumisen yhteydessä Office 2016:n koontiversioon 16.0.7967 Windows 10:ssä](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Officen toinen tili on jo kirjautunut sisään tähän tietokoneeseen"](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Officen nykyaikaisen todennuksen kirjautumisongelmien vianmääritys ADFS:ää käytettäessä](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)