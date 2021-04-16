---
title: Aktivointiongelma – Yhteyttä ei voida muodostaa juuri nyt
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
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806439"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Microsoft 365 -sovellusten "Yhteyttä ei voida juuri nyt" -viestin asentaminen

Jos näyttöön tulee tämä sanoma, kokeile seuraavaa:

1. Tarkista palomuurin, virustentorjuntaohjelman ja välityspalvelimen asetukset ja varmista, että ne eivät estä Microsoft 365 -sovellusten Internet-yhteyttä. Katso [Microsoftin URL-osoitteet ja IP-osoitealueet.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Siirry Käynnistä **Suorita**  >  **-valikkoon** ja kirjoita **services.msc.** Varmista, että seuraavat palvelut ovat käynnissä:
    - Verkkoon yhdistetyt laitteet – automaattinen määritys
    - Verkkoluettelopalvelu
    - Verkkosijainnin tietoisuus
    - Windowsin tapahtumaloki

Jos jokin näistä palveluista ei ole käynnissä, yritä käynnistää se. Jos palvelun avaamisessa ilmenee ongelmia, suorita seuraava komento avaamalla komentokehote, jossa on järjestelmänvalvojan oikeudet:

**sfc /scannow**

Kun tämä komento on valmis, käynnistä tietokone uudelleen.

Lisätietoja on [kohdassa "Tiliisi ei voi muodostaa yhteyttä. Yritä myöhemmin uudelleen"-virhe aktivoitaessa Officen Microsoft 365:stä.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)