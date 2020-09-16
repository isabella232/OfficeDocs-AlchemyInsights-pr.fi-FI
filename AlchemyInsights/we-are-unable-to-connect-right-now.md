---
title: Aktivointi ongelma – yhteyden muodostaminen ei onnistu juuri nyt
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725980"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Microsoft 365-sovellusten korjaaminen "emme pysty muodostamaan yhteyttä juuri nyt"-viesti

Jos saat tämän viestin, kokeile seuraavaa:

1. Tarkista palo muurin, virustentorjuntaohjelman ja välitys palvelimen asetukset ja varmista, että ne eivät estä Internet-yhteyttä Microsoft 365-sovelluksiin. Katso [Microsoftin URL-osoitteet ja IP-osoite alueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Siirry **Käynnistä**  >  **Suorita**-kohtaan ja kirjoita **Services. msc**. Varmista, että seuraavat palvelut ovat käynnissä:
    - Verkkoon yhdistetyt laitteet automaattinen määritys
    - Verkko luettelon palvelu
    - Verkko sijainnin tietoisuus
    - Windowsin tapahtuma loki

Jos jokin näistä palveluista ei ole käynnissä, yritä käynnistää se. Jos sinulla on ongelmia palvelun aloittamisessa, suorita seuraava komento avaamalla komento kehote laajenne tuilla käyttö oikeuksilla:

**SFC/scannow**

Kun tämä komento on valmis, Käynnistä tieto kone uudelleen.

Katso lisä tietoja kohdasta ["Pahoittelemme, emme voi muodostaa yhteyttä tiliisi. Yritä uudelleen myöhemmin-virhe, kun Akti voit Officen Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)-versiosta.