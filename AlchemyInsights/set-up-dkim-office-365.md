---
title: DKIM:n määrittäminen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645669"
---
# <a name="setup-dkim"></a>DKIM:n määrittäminen

Täydelliset ohjeet DKIM:n määrittämiseen microsoft 365:n mukautetuille toimialueille ovat [täällä](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. **Jokaiselle** mukautetulle toimialueelle on luotava **kaksi** DKIM CNAME -tietuetta toimialueen DNS-isännöintipalveluun (yleensä toimialueen rekisteröintipalveluun). Esimerkiksi contoso.com ja fourthcoffee.com edellyttää neljää DKIM CNAME -tietuetta: kaksi contoso.com ja kaksi fourthcoffee.com.

   **Kunkin** mukautetun toimialueen DKIM CNAME -tietueet käyttävät seuraavia muotoja:

   - **Isännän nimi**:`selector1._domainkey.<CustomDomain>`

     **Osoite- tai arvopisteet:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **Kävi koulua TTL**: 3600

   - **Isännän nimi**:`selector2._domainkey.<CustomDomain>`

     **Osoite- tai arvopisteet:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **Kävi koulua TTL**: 3600

   \<DomainGUID\> on mukautetun toimialueen `.mail.protection.outlook.com` mukautetun MX-tietueen (esimerkiksi `contoso-com` toimialueen contoso.com) mukautetun MX-tietueen vasemmalla puolella oleva teksti. \<InitialDomain\> on toimialue, jota käytit rekisteröityessäsi Microsoft 365:een (esimerkiksi contoso.onmicrosoft.com).

2. Kun olet luonut Mukautettujen toimialueiden CNAME-tietueet, toimi seuraavasti:

   A. [kirjaudu Microsoft 365:een](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) työpaikan tai oppilaitoksen tilillä.

   B. Valitse vasemmasta yläkulmasta sovellusten käynnistyskuvake ja valitse **Järjestelmänvalvoja**.

   C. Laajenna vasemmassa alakulmassa **Järjestelmänvalvoja** ja valitse **Exchange**.

   D. Siirry **Kohtaan Suojaus** > **DKIM**.

   E. Valitse toimialue ja valitse sitten **Ota käyttöön** tämän **toimialueen Sign-viesteille DKIM-allekirjoituksilla**. Toista tämä vaihe jokaisen mukautetun toimialueen kohdalla.
