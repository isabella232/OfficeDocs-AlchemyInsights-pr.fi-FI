---
title: Suojaus backscatter-hyökkäyksiltä
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035412"
---
# <a name="protection-from-backscatter-attack"></a>Suojaus backscatter-hyökkäyksiltä

Katkosviestit ovat toimituksen ilmoituksia (ns. NNR-ilmoituksia tai viestin toimituksen toimitusilmoituksia), joita vastaanotat viesteistä, joita et ole lähettänyt. Roskapostin lähettämien estoviestien **vastaanottaja:** viestien osoite, ja ne käyttävät usein oikeita sähköpostiosoitteita uskottavuuden lisäämiseksi viesteilleen. Kun roskapostin lähettäjät lähettävät viestejä väistämättä ei-olemassa olevalle vastaanottajalle, kohdesähköpostipalvelinta huijataan palauttamaan NDR-viesti lähettäjälle **Lähettäjä:-osoitteessa.**

Lisätietoja on [EOP:n backscatter-kohdassa.](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)

**Taustasuojauksen ottaminen käyttöön**

Jos haluat ottaa käyttöön taustasuojauksen, noudata alla olevaa polkua.

**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to "On"**

Jos uskot, että tili on vaarantunut, katso seuraavat:

- [Vaarannun sähköpostitiliin vastaaminen](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [Estettyjen käyttäjien poistaminen Office 365:n Rajoitetut käyttäjät -portaalista](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



