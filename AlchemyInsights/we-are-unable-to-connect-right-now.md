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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716169"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Office-sovellusten korjaaminen "Emme pysty muodostamaan yhteyttä juuri nyt" -sanoma

Jos saat tämän sanoman, kokeile seuraavaa:

1. Tarkista palomuurin, virustentorjuntaohjelmiston ja välityspalvelimen asetukset ja varmista, että ne eivät estä Office-sovellusten Internet-yhteyttä. Lisätietoja on [ohjeaiheessa Microsoftin URL-osoitteet ja IP-osoitealueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Siirry **Käynnistä-kohtaan** > **Run**ja kirjoita **services.msc**. Varmista, että seuraavat palvelut ovat käynnissä:
    - Verkkoon liitettyjen laitteiden automaattinen asennus
    - Verkkoluettelopalvelu
    - Verkon sijaintitietoisuus
    - Windowsin tapahtumaloki

Jos jokin näistä palveluista ei ole käynnissä, yritä käynnistää se. Jos palvelun käynnistämisessä on ongelmia, suorita seuraava komento avaamalla komentorivi, jolla on laajennetut käyttöoikeudet:

**Kävi koulua sfc /scannow**

Kun tämä komento on valmis, käynnistä tietokone uudelleen.

Lisätietoja on kohdassa ["Valitettavasti emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen" -virhe, kun aktivoit Officen Microsoft 365:stä.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)