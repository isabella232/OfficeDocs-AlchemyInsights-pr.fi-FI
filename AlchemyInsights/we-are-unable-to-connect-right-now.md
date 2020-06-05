---
title: Aktivointiongelma - Emme pysty muodostamaan yhteyttä juuri nyt
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581872"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Microsoft 365 -sovellusten "Emme pysty muodostamaan yhteyttä juuri nyt" -sanoman korjaaminen

Jos näyttöön tulee tämä sanoma, kokeile seuraavaa:

1. Tarkista palomuurin, virustentorjuntaohjelmiston ja välityspalvelimen asetukset ja varmista, että ne eivät estä Microsoft 365 -sovellusten Internet-käyttöä. Lisätietoja [on kohdassa Microsoftin URL-osoitteet ja IP-osoitealueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Siirry **Käynnistä**  >  **Suorita**ja kirjoita **services.msc**. Varmista, että kaikki seuraavat palvelut ovat käynnissä:
    - Verkkoon liitettyjen laitteiden automaattinen asennus
    - Verkkoluettelopalvelu
    - Verkon sijainnin tunnettuus
    - Windowsin tapahtumaloki

Jos jokin näistä palveluista ei ole käynnissä, yritä käynnistää se. Jos palvelun käynnistämisessä on ongelmia, suorita seuraava komento avaamalla komentorivi, jolla on laajennetut käyttöoikeudet:

**sfc / scannow**

Kun tämä komento on valmis, käynnistä tietokone uudelleen.

Lisätietoja on [ohjeaiheessa "Emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen -virhe, kun aktivoit Officen Microsoft 365:stä.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)