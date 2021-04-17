---
title: Microsoft 365 -sovellusten asentaminen Valitettavasti Tilapäiset palvelinongelmat -viesti
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
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835268"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Microsoft 365 -sovellusten "Tilapäiset palvelinongelmat valitettavasti" -viestin asentaminen

Jos näyttöön tulee tämä sanoma, kokeile seuraavaa:

1. Tarkista palomuurin, virustentorjuntaohjelman ja välityspalvelimen asetukset ja varmista, että ne eivät estä Microsoft 365 -sovellusten Internet-yhteyttä. Katso [URL-osoitteet ja IP-osoitealueet.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Siirry Käynnistä **Suorita**  >  **-valikkoon** ja kirjoita **services.msc.** Varmista, että seuraavat palvelut ovat käynnissä:
    - Verkkoon yhdistetyt laitteet – automaattinen määritys
    - Verkkoluettelopalvelu
    - Verkkosijainnin tietoisuus
    - Windowsin tapahtumaloki

Jos jokin näistä palveluista ei ole käynnissä, yritä käynnistää se. Jos palvelun avaamisessa ilmenee ongelmia, suorita seuraava komento avaamalla komentokehote, jossa on järjestelmänvalvojan oikeudet:

**sfc /scannow**

Kun tämä komento on valmis, käynnistä tietokone uudelleen.

Lisätietoja on [kohdassa "Tiliisi ei voi muodostaa yhteyttä. Yritä myöhemmin uudelleen"-virhe aktivoitaessa](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).