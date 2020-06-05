---
title: Microsoft 365 -sovellusten korjaaminen Anteeksi, meillä on tilapäisiä palvelinongelmia -sanoma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582700"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Microsoft 365 -sovellusten korjaaminen "Anteeksi, meillä on tilapäisiä palvelinongelmia" -sanoma

Jos näyttöön tulee tämä sanoma, kokeile seuraavaa:

1. Tarkista palomuurin, virustentorjuntaohjelmiston ja välityspalvelimen asetukset ja varmista, että ne eivät estä Microsoft 365 -sovellusten Internet-käyttöä. Katso [URL-osoitteet ja IP-osoitealueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Siirry **Käynnistä**  >  **Suorita**ja kirjoita **services.msc**. Varmista, että kaikki seuraavat palvelut ovat käynnissä:
    - Verkkoon liitettyjen laitteiden automaattinen asennus
    - Verkkoluettelopalvelu
    - Verkon sijainnin tunnettuus
    - Windowsin tapahtumaloki

Jos jokin näistä palveluista ei ole käynnissä, yritä käynnistää se. Jos palvelun käynnistämisessä on ongelmia, suorita seuraava komento avaamalla komentorivi, jolla on laajennetut käyttöoikeudet:

**sfc / scannow**

Kun tämä komento on valmis, käynnistä tietokone uudelleen.

Lisätietoja on [ohjeaiheessa "Emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen -virhe, kun aktivoit](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).