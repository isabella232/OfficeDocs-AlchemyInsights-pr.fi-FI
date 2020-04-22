---
title: Roskapostin esto - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676494"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Korjaa sähköpostin toimitusongelmat virhekoodille 5.7.23

Tarkista toimialueesi SPF-DNS-tietue verkossa julkisesti saatavilla olevassa SPF- tai DNS-tietueen tarkistuksessa.

Varmista, että Microsoft ei tunnistanut lähtevää viestiä roskapostiksi ja että se reititetään [suuren riskin toimituspoolin](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages)kautta. Suuren riskin toimituspoolissa olevat viestit eivät läpäise SPF-tarkistuksia, joten kohdesähköpostiorganisaatio ei hyväksy niitä.

Jos ongelma ei poistu, sinun on ehkä otettava yhteyttä sen sähköpostiisännän järjestelmänvalvojaan, johon yrität lähettää sähköpostia. Merkitse muistisanomassa käytettävissä oleva yksityiskohtainen ulkoinen virhe muistiin. Microsoftin tuki ei ehkä voi auttaa enempää.
