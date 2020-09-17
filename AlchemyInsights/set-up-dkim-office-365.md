---
title: Setup DKIM
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
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808704"
---
# <a name="setup-dkim"></a>Setup DKIM

Microsoft 365: n mukautettujen toimi alueiden DKIM-määrityksen täydelliset ohjeet ovat [täällä](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. Sinun on luotava **kullekin** mukautetulle toimi alueelle **kaksi** DKIM CNAME-tietuetta toimi alueen DNS-isännöinti palvelussa (yleensä toimi alueen rekisteröinti palvelu). Esimerkiksi contoso.com ja fourthcoffee.com vaativat neljä DKIM CNAME-tietuetta: kaksi contoso.com ja kaksi fourthcoffee.com.

   **Kunkin** mukautetun toimi alueen DKIM CNAME-tietueet käyttävät seuraavia muotoiluja:

   - **Isäntä nimi**: `selector1._domainkey.<CustomDomain>`

     **Osoittaa osoitteen tai arvon**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Isäntä nimi**: `selector2._domainkey.<CustomDomain>`

     **Osoittaa osoitteen tai arvon**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> on `.mail.protection.outlook.com` mukautetun toimi alueen mukautetun MX-tietueen (esimerkiksi `contoso-com` toimi alueen contoso.com) vasemmalla puolella oleva teksti. \<InitialDomain\> on toimi alue, jota käytit rekisteröityessäsi Microsoft 365-käyttöön (esimerkiksi contoso.onmicrosoft.com).

2. Kun olet luonut mukautettujen toimi alueiden CNAME-tietueet, noudata seuraavia ohjeita:

   a. [Kirjaudu sisään Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) työpaikan tai oppi laitoksen tilillä.

   b. Valitse vasemmasta yläkulmasta sovellusten käynnistyskuvake ja valitse **Järjestelmänvalvoja**.

   c. Laajenna vasemmassa alakulmassa olevaa siirtymis ruudussa **järjestelmänvalvoja** -kohtaa ja valitse **Exchange**.

   d. Siirry kohtaan **Suojaus**-  >  **DKIM**.

   e. Valitse toimi alue ja valitse sitten **Ota käyttöön** **tämän toimi alueen allekirjoita viestit DKIM-allekirjoituksilla**. Toista tämä vaihe kunkin mukautetun toimi alueen kohdalla.
