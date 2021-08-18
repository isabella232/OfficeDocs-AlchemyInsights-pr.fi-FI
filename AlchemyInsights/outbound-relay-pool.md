---
title: Lähtevien välitysen välitysalue
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: 7e5bb1fda1dec0c0f72d1944d54b6f2747a6e909
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326074"
---
# <a name="outbound-relay-pool"></a>Lähtevien välitysen välitysalue

Microsoft tekee joitakin muutoksia sähköpostiviestien välityksen tai edelleenlähetysmäärityksen Microsoft 365. Tietyissä tilanteissa viestit välitetään tai välitetään Microsoft 365 erityisen välitystilan avulla. Välityksen avulla lähetetyt viestit voivat päätyä vastaanottajan roskapostikansioon. Lisätietoja on kohdassa Lähtevät [toimituslähteet](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Jos haluat välttää skenaarion käyttää välityksen välitysä, varmista, että edelleen lähetetyt/välitetut viestit täyttävät yhden seuraavista ehdoista:

- Lähtevä lähettäjä on vuokraajan hyväksytty toimialue.
- SPF (Sender Policy Framework) välittää viestin, kun viesti Microsoft 365.
- P2-lähettäjän toimialueen DomainKeys Identified Mail (DKIM) -näppäin vastaa viestin Microsoft 365.
 
Viestejä, jotka täyttävät edellä mainitut ehdot, ei välitetä välityksen kautta.

Jos toimialueesi MX-tietue osoittaa kolmannen osapuolen tai paikallisen palvelimen, varmista laajennetun suodatuksen avulla, että SPF-vahvistus on oikea saapuvalle sähköpostille, eikä sähköpostia lähetetä välityksen kautta.

**Miten voimme tietää, vaikuttaako välitysalue meitä?**

Jos välitetyissä tai välitetyissä sähköpostiviesteissä käytetään jotain yllä mainituista ehdoista, viestejä ei välitetä välityksen kautta. Jos viesti lähetetään välitysalueen kautta, lähtevän postin palvelimen IP-osoite on 40.95.0.0/16-alueella ja lähtevän liikenteen palvelimen nimi **näkyy nimenä rly.**

