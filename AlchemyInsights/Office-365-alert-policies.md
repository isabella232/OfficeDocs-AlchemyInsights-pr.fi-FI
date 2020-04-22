---
title: 1385-Office-365-hälytyskäytännöt
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 1209e59668bbe69fe88408933ae11b357b8d4f1a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687615"
---
# <a name="alert-policies"></a>Hälytyskäytännöt

Microsoft 365:n tietoturva& Compliance Center issä on [oletushälytyskäytäntöjä,](https://docs.microsoft.com/office365/securitycompliance/alert-policies#default-alert-policies) jotka käynnistävät hälytykset organisaatioille, joilla on Office 365 Enterprise- tai Office 365 US Government E1/G1-, E3/G3- tai E5/G5-tilaus. Tämän vuoksi järjestelmänvalvojat voivat saada Office365Alerts@microsoft.com lähettämän ilmoitusilmoituksen, jonka aiherivi on "Matalan vakavuusilmoituksen: *hälytyskäytännön nimi".* Hälytysilmoitukset lähetetään, kun hälytyksiä käynnistetään yleisille toiminnoille, esimerkiksi silloin, kun käyttäjät:

- Luo saapuneet-kansion sääntöjä, jotka välittävät sähköpostia.
- Määritä postilaatikon käyttöoikeudet.
- Jaa tai poista suuri määrä tiedostoja SharePoint-tiedostojen jakamisessa.
- Luo eDiscovery-hakuja ja vie hakutulokset.

Hälytyksen tarkistaminen ja sen mukaan toimiminen:

1. Siirry [Suojaus-& yhteensopivuuskeskukseen](https://protection.office.com) ja kirjaudu sisään.
2. Valitse **Hälytykset** > **Näytä hälytykset**.
3. Napsauttamalla ilmoitusta saat näkyviin pikaikkunasivun, jossa on tietoja ilmoituksesta.

Voit tehdä hälytyksen toimia, kuten [poistaa epäilyttävän Saapuneet-kansion säännön](https://docs.microsoft.com/office365/securitycompliance/responding-to-a-compromised-email-account). Voit myös sulkea ilmoituksen valitsemalla hälytyspikaikkunasivulla **Ratkaise.**

Lisätietoja hälytyskäytäntöjen määrittämisestä ja hallinnasta on [tässä artikkelissa](https://docs.microsoft.com/office365/securitycompliance/alert-policies).

**Tärkeää**: Microsoftin sähköposti-ilmoitukset eivät koskaan pyydä sinua tekemään seuraavaa:

- Salasanan anto
- Tilin suojaustietojen vahvistaminen
- Vahvista itsesi uudelleen

Jos saat sähköpostiviestin näin, Microsoft ei lähettänyt sitä, ja sitä tulisi pitää tietojenkalasteluhuijauksena. Jos näin tapahtuu, [ilmoita siitä Microsoftille](https://docs.microsoft.com/office365/SecurityCompliance/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).