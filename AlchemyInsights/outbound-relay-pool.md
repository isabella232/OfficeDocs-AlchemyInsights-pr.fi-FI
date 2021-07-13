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
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381713"
---
# <a name="outbound-relay-pool"></a>Lähtevien välitysen välitysalue

Microsoft tekee joitakin muutoksia sähköpostien välityksen tai edelleenlähetysmäärityksen Microsoft 365. Tietyissä tilanteissa viestit välitetään tai välitetään Microsoft 365 erityisen välitystilan avulla. Välityksen avulla lähetetyt viestit voivat päätyä vastaanottajan roskapostikansioon. Lisätietoja on kohdassa Lähtevät [toimituslähteet](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Voit välttää skenaarion käyttämällä välityksen välitysä varmistamalla, että välitettyjen/välitettyjen viestien on täytettävä jokin seuraavista ehdoista:

- Lähtevä lähettäjä on vuokraajan hyväksytty toimialue.
- SPF (Sender Policy Framework) välittää viestin, kun viesti Microsoft 365.
- P2-lähettäjän toimialueen DomainKeys Identified Mail (DKIM) -näppäin vastaa viestin Microsoft 365.
 
Viestejä, jotka täyttävät edellä mainitut ehdot, ei välitetä välityksen kautta.

Jos toimialueesi MX-tietue osoittaa kolmannen osapuolen tai paikallisen palvelimen, varmista laajennetun suodatuksen avulla, että SPF-vahvistus on oikea saapuvalle sähköpostille, eikä sähköpostia lähetetä välityksen kautta.

**Miten voimme tietää, vaikuttaako välitysalue meitä?**

Jos välitetyissä tai välitetyissä sähköpostiviesteissä käytetään jotain edellä mainituista ehdoista, viestejä ei välitetä välityksen kautta. Jos viesti lähetetään välityspalvelimen kautta, lähtevän palvelimen IP-osoite on 40.95.0.0/16-alueella ja lähtevän postin palvelimen nimi **näkyy nimenä rly.**

