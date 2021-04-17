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
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821408"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Sähköpostin toimitusongelman korjaus virhekoodille 5.7.23

Tarkista toimialueen SPF DNS -tietue internetissä yleisesti saatavilla olevan SPF- tai DNS-tietueiden tarkistuspalvelun kautta.

Varmista, että Microsoft ei ole tunnistanut lähtevää viestiä roskapostiksi ja että se reititettiin Suuren riskin [toimitus poolin kautta.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Suuren riskin toimitus poolin viestit eivät läpäise SPF-tarkistuksia, joten kohdesähköpostiorganisaatio ei hyväksy niitä.

Jos ongelma jatkuu, sinun on ehkä otettava yhteyttä sen sähköpostipalvelimen järjestelmänvalvojaan, jolle yrität lähettää sähköpostia. Merkitse yksityiskohtainen ulkoinen virhe muistiin ilmoituksen ilmoitusviestin ilmoituksista. Microsoft-tuki ei ehkä voi auttaa enempää.
