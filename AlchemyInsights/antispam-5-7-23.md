---
title: Roskaposti - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932166"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Sähköpostin toimitusongelman korjaus virhekoodille 5.7.23

Tarkista toimialueen SPF DNS -tietue internetissä yleisesti saatavilla olevan SPF- tai DNS-tietueiden tarkistuspalvelun kautta.

Varmista, että Microsoft ei ole tunnistanut lähtevää viestiä roskapostiksi ja että se reititettiin Suuren riskin [toimitus poolin kautta.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Suuren riskin toimitus poolin viestit eivät läpäise SPF-tarkistuksia, joten kohdesähköpostiorganisaatio ei hyväksy niitä.

Jos ongelma jatkuu, sinun on ehkä otettava yhteyttä sen sähköpostipalvelimen järjestelmänvalvojaan, jolle yrität lähettää sähköpostia. Merkitse yksityiskohtainen ulkoinen virhe muistiin ilmoituksen ilmoitusviestin ilmoituksista. Microsoft-tuki ei ehkä voi auttaa enempää.
