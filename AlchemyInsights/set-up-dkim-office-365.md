---
title: DKIM:n määrittäminen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108553"
---
# <a name="setup-dkim"></a>DKIM:n määrittäminen

Täydelliset ohjeet DKIM:n määrittämiseen mukautettuja toimialueita varten Microsoft 365 [ovat täällä.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. Jokaiselle **mukautetulle** toimialueelle on luotava kaksi **DKIM** CNAME -tietuetta toimialueen DNS-isännöintipalveluun (yleensä toimialuerekisteröijä). Esimerkiksi contoso.com ja fourthcoffee.com edellyttää neljäÄ DKIM CNAME -tietuetta: kaksi contoso.com ja kaksi fourthcoffee.com.

   Kunkin mukautetun toimialueen DKIM CNAME **-tietueet** käyttävät seuraavia muotoja:

   - **Isäntänimi:**`selector1._domainkey.<CustomDomain>`

     **Osoittaa osoitteeseen tai arvoon:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Isäntänimi:**`selector2._domainkey.<CustomDomain>`

     **Osoittaa osoitteeseen tai arvoon:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> on mukautetun toimialueen mukautetun MX-tietueen (esimerkiksi toimialueen tai toimialueen) `.mail.protection.outlook.com` `contoso-com` mukautetun MX-tietueen vasemmalla contoso.com). \<InitialDomain\>on toimialue, jota käytit rekisteröityessäsi Microsoft 365 (esimerkiksi contoso.onmicrosoft.com).

2. Kun olet luonut CNAME-tietueet mukautettuja toimialueita varten, toimi seuraavasti:

   a. [kirjaudu sisään Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) tai koulun tilillä.

   b. Valitse vasemmasta yläkulmasta sovellusten käynnistyskuvake ja valitse **Järjestelmänvalvoja**.

   c. Laajenna vasemman alakulman siirtymisruudussa **Järjestelmänvalvoja** ja **valitse Exchange**.

   d. Siirry **Protection**  >  **DKIM (Suojaus DKIM) -ruudulle.**

   e. Valitse toimialue ja valitse sitten **Sign** messages for this domain with DKIM signatures (Allekirjoita tämän toimialueen viestit **DKIM-allekirjoituksella) -kohdassa Ota käyttöön.** Toista tämä vaihe jokaisen mukautetun toimialueen yhteydessä.
