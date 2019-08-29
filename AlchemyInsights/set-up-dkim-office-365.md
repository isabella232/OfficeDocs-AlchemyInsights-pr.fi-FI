---
title: 'Asennus DKIM Office 365: ssä'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666261"
---
# <a name="setup-dkim-in-office-365"></a>Asennus DKIM Office 365: ssä

DKIM määrittäminen Office 365: ssä mukautetut toimialueet ovat täydelliset ohjeet [tähän](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. **Kutakin** mukautettua toimialuetta täytyy luoda **kaksi** DKIM CNAME-tietueita toimialueen DNS-sivustotilapalvelun (yleensä toimialueen registrar). Esimerkiksi contoso.com ja fourthcoffee.com vaativat neljä DKIM CNAME-tietueet: contoso.com ja kaksi fourthcoffee.com, kaksi.

   **Kutakin** mukautettua toimialuetta DKIM CNAME-tietueita käytetään seuraavissa muodoissa:

   - **Isännän nimi**:`selector1._domainkey.<CustomDomain>`

     **Osoite tai arvo viittaa**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Isännän nimi**:`selector2._domainkey.<CustomDomain>`

     **Osoite tai arvo viittaa**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> on teksti vasemmalla puolella `.mail.protection.outlook.com` mukautetut MX-tietueen mukautetun toimialueen (esimerkiksi `contoso-com` , toimialueen contoso.com). \<InitialDomain\> on toimialue, jota käytit Kun rekisteröidyit Office 365 (esimerkiksi contoso.onmicrosoft.com) varten.

2. Kun olet luonut CNAME-tietueet, mukautettujen toimialueiden, toimimalla seuraavien ohjeiden mukaan:

   a. [Kirjaudu Office 365:een](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) antamalla työpaikan tai oppilaitoksen tili.

   b. Valitse vasemmasta yläkulmasta sovellusten käynnistyskuvake ja valitse **Järjestelmänvalvoja**.

   c. Vasemmassa siirtymispalkissa Laajenna **Admin** ja valitse **Exchange**.

   d. Siirry **Suojaa** > **DKIM**.

   e. Valitse toimialue ja valitse sitten **merkki**viesteissä DKIM-allekirjoituksia sisältävien tämän toimialueen **käyttöön** . Toista tämä vaihe kunkin mukautetun toimialueen.
