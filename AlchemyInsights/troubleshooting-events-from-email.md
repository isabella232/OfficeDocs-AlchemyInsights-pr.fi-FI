---
title: Sähköpostitapahtumien vianmääritys
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834836"
---
# <a name="troubleshooting-events-from-email"></a>Sähköpostitapahtumien vianmääritys

1. Tarkista, että ominaisuus on otettu käyttöön postilaatikossa: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Katso sitten Tapahtumat sähköpostista -lokeja **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Etsi Tapahtumat sähköpostista -lokeihin InternetMessageId, joka vastaa postilaatikon kohdetta.  

4. TrustScore määrittää, lisätäänkö kohde vai ei. Tapahtumat lisätään vain, jos TrustScore = "Luotettu".

TrustScore määritetään SPF-, Dkim- tai Dmarc-ominaisuuksien mukaan, jotka ovat viestin otsikossa.

Voit tarkastella näitä ominaisuuksia seuraavasti:

**Outlookin työpöytäversio**

- Avaa kohde
- Tiedosto -> -> Internet-otsikot

TAI

**MFCMapi**

- Siirtyminen Saapuneet-kansion kohteeseen
- Etsi PR_TRANSPORT_MESSAGE_HEADERS_W

Nämä ominaisuudet määritetään ja tallennetaan reitityksen ja reitityksen aikana. Jos tarvitset lisää vianmääritystä, sinun on ehkä seurattava siirtotukea SPF-, DKIM- ja DMARC-virheistä.