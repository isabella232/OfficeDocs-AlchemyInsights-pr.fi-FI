---
title: Aktivointi ongelma-emme voi muodostaa yhteyttä juuri nyt
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
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628239"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Office-sovellusten korjaaminen "emme pysty yhdistämään juuri nyt"-viestiä

Jos tämä sanoma tulee näyttöön, kokeile seuraavia:

1. Tarkista palo muuri-, virustentorjuntaohjelmisto-ja välitys palvelin asetukset ja varmista, etteivät ne estä Internet-pääsyä Office-sovelluksiin. Katso [Office 365-URL-osoitteet ja IP-osoite alueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Siirry kohtaan **Aloita** > **suorittaminen**ja kirjoita **Services. msc**. Varmista, että seuraavat palvelut ovat käynnissä:
    - Verkkoon liitettyjen laitteiden automaattinen määritys
    - Verkko luettelo palvelu
    - Verkon sijainti tietoisuus
    - Windowsin tapahtuma loki

Jos jokin näistä palveluista ei ole käynnissä, yritä käynnistää se. Jos sinulla on ongelmia palvelun käynnistettäessä, suorita seuraava komento avaamalla komento kehote, jossa on laajennettuja käyttö oikeuksia:

**SFC/scannow**

Kun tämä komento on suoritettu, Käynnistä tieto kone uudelleen.

Lisä tietoja on kohdassa ["anteeksi, emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen "-virhe, kun Akti voit Officen Office-365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).