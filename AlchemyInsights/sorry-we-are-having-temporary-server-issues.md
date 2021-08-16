---
title: Korjaus Microsoft 365-sovelluksiin Valitettavasti tilapäiset palvelinongelmat on viesti
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
- "3420"
- "9001430"
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021593"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Viestin Microsoft 365 "Valitettavasti tilapäiset palvelinongelmat" -viesti

Jos näyttöön tulee tämä sanoma, kokeile seuraavaa:

1. Tarkista palomuurin, virustentorjuntaohjelman ja välityspalvelimen asetukset ja varmista, että ne eivät estä Microsoft 365 internet-yhteyttä. Katso [URL-osoitteet ja IP-osoitealueet.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Siirry Käynnistä **Suorita**  >  **-valikkoon** ja kirjoita **services.msc.** Varmista, että seuraavat palvelut ovat käynnissä:
    - Verkkoon yhdistetyt laitteet – automaattinen määritys
    - Verkkoluettelopalvelu
    - Verkkosijainnin tietoisuus
    - Windows Tapahtumaloki

Jos jokin näistä palveluista ei ole käynnissä, yritä käynnistää se. Jos palvelun avaamisessa ilmenee ongelmia, suorita seuraava komento avaamalla komentokehote, jossa on järjestelmänvalvojan oikeudet:

**sfc /scannow**

Kun tämä komento on valmis, käynnistä tietokone uudelleen.

Lisätietoja on [kohdassa "Tiliisi ei voi muodostaa yhteyttä. Yritä myöhemmin uudelleen"-virhe aktivoitaessa](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).