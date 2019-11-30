---
title: Office-sovellusten korjaaminen anteeksi, meillä on väliaikainen palvelin ongelmien viesti
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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627987"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Office-sovellusten korjaaminen "Valitettavasti meillä on tilapäisiä palvelin ongelmia"-viesti

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