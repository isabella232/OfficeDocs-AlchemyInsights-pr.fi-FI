---
title: Fixing Microsoft 365-sovellukset Pahoittelemme, meillä on väliaikainen palvelin ongelmien viesti
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758242"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Microsoft 365-sovellusten korjaaminen "Valitettavasti meillä on väliaikaisia palvelin ongelmia"-viesti

Jos saat tämän viestin, kokeile seuraavaa:

1. Tarkista palo muurin, virustentorjuntaohjelman ja välitys palvelimen asetukset ja varmista, että ne eivät estä Internet-yhteyttä Microsoft 365-sovelluksiin. Katso [URL-osoitteet ja IP-osoite alueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Siirry **Käynnistä**  >  **Suorita**-kohtaan ja kirjoita **Services. msc**. Varmista, että seuraavat palvelut ovat käynnissä:
    - Verkkoon yhdistetyt laitteet automaattinen määritys
    - Verkko luettelon palvelu
    - Verkko sijainnin tietoisuus
    - Windowsin tapahtuma loki

Jos jokin näistä palveluista ei ole käynnissä, yritä käynnistää se. Jos sinulla on ongelmia palvelun aloittamisessa, suorita seuraava komento avaamalla komento kehote laajenne tuilla käyttö oikeuksilla:

**SFC/scannow**

Kun tämä komento on valmis, Käynnistä tieto kone uudelleen.

Katso lisä tietoja kohdasta ["Pahoittelemme, emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen-virhe aktivoitaessa](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).