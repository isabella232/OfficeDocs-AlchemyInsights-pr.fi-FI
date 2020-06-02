---
title: Roskapostin torjunta - 5.7.23
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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506440"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Virhekoodin 5.7.23 sähköpostin toimitusongelmien korjaaminen

Tarkista toimialueesi SPF DNS -tietue julkisesti saatavilla olevasta SPF- tai DNS-tietueiden tarkistamisesta verkossa.

Varmista, että Microsoft ei tunnistanut lähtevää viestiä roskapostiksi ja että se reititetään [suuren riskin toimitusvarannon](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)kautta. Suuren riskin toimitusvarannon viestit eivät läpäise SPF-tarkistuksia, joten kohdesähköpostiorganisaatio ei hyväksy niitä.

Jos ongelma ei poistu, sinun on ehkä otettava yhteyttä sen sähköpostiisännän järjestelmänvalvojaan, johon yrität lähettää sähköpostia. Merkitse muistiin poistumisviestissä käytettävissä oleva yksityiskohtainen ulkoinen virhe. Microsoftin tuki ei ehkä voi auttaa enempää.
