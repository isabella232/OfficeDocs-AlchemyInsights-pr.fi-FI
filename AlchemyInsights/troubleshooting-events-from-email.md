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
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105349"
---
# <a name="troubleshooting-events-from-email"></a>Sähköpostitapahtumien vianmääritys

1. Tarkista, että ominaisuus on otettu käyttöön postilaatikossa: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Katso sitten Tapahtumat sähköpostista -lokeja **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Etsi Tapahtumat sähköpostista -lokeihin InternetMessageId, joka vastaa postilaatikon kohdetta.  

4. TrustScore määrittää, lisätäänkö kohde vai ei. Tapahtumat lisätään vain, jos TrustScore = "Luotettu".

TrustScore määritetään SPF-, Dkim- tai Dmarc-ominaisuuksien mukaan, jotka ovat viestin otsikossa.

Voit tarkastella näitä ominaisuuksia seuraavasti:

**Työpöytä Outlook**

- Avaa kohde
- Tiedosto -> -> Internet-otsikot

TAI

**MFCMapi**

- Siirtyminen Saapuneet-kansion kohteeseen
- Etsi PR_TRANSPORT_MESSAGE_HEADERS_W

Nämä ominaisuudet määritetään ja tallennetaan reitityksen ja reitityksen aikana. Jos tarvitset lisää vianmääritystä, sinun on ehkä seurattava siirtotukea SPF-, DKIM- ja DMARC-virheistä.