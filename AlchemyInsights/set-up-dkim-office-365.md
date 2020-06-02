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
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509381"
---
# <a name="setup-dkim"></a>DKIM:n määrittäminen

Täydelliset ohjeet DKIM:n määrittämiseen microsoft 365:n mukautetuille toimialueille ovat [täällä](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. **Jokaiselle** mukautetulle toimialueelle on luotava **kaksi** DKIM CNAME -tietuetta toimialueen DNS-isännöintipalvelussa (yleensä toimialueen rekisteröintipalvelu). Esimerkiksi contoso.com ja fourthcoffee.com vaativat neljä DKIM CNAME -tietuetta: kaksi contoso.com ja kaksi fourthcoffee.com.

   **Kunkin** mukautetun toimialueen DKIM CNAME -tietueissa käytetään seuraavia muotoja:

   - **Isännän nimi**:`selector1._domainkey.<CustomDomain>`

     **Osoite- tai arvopisteet:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600 (alv.)

   - **Isännän nimi**:`selector2._domainkey.<CustomDomain>`

     **Osoite- tai arvopisteet:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600 (alv.)

   \<DomainGUID\>on mukautetun toimialueen mukautetun MX-tietueen vasemmalla puolella oleva teksti `.mail.protection.outlook.com` (esimerkiksi `contoso-com` toimialueen contoso.com). \<InitialDomain\>on toimialue, jota käytit rekisteröityessäsi Microsoft 365:ään (esimerkiksi contoso.onmicrosoft.com).

2. Kun olet luonut CNAME-tietueet mukautetuille toimialueillesi, toimi seuraavasti:

   a. [kirjaudu Microsoft 365:lle](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) työpaikan tai oppilaitoksen tilillä.

   b. Valitse vasemmasta yläkulmasta sovellusten käynnistyskuvake ja valitse **Järjestelmänvalvoja**.

   c. Laajenna vasemmassa alakulmassa **Järjestelmänvalvoja** ja valitse **Exchange**.

   D. Siirry **Protection**  >  **DKIM**.

   E. Valitse toimialue ja valitse sitten **Ota käyttöön** tämän **toimialueen allekirjoita-viesteissä DKIM-allekirjoituksilla**. Toista tämä vaihe jokaisen mukautetun toimialueen kohdalla.
