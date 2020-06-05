---
title: Tapahtumien vianmääritys sähköpostista
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569143"
---
# <a name="troubleshooting-events-from-email"></a>Tapahtumien vianmääritys sähköpostista

1. Varmista, että ominaisuus on otettu käyttöön postilaatikossa: **Get-EventsFromEmailConfiguration -Identity <mailbox> **

2. Katso sitten "Tapahtumat sähköpostista" lokit **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Etsi Sähköpostitapahtumat-lokit -lokista internetmessageId, joka vastaa postilaatikon kohdetta.  

4. TrustScore määrittää, lisätäänkö kohde vai ei. Tapahtumat lisätään vain, jos TrustScore = "Luotettu".

TrustScore määräytyy SPF-, Dkim- tai Dmarc-ominaisuuksien mukaan, jotka ovat viestin otsikossa.

Voit tarkastella näitä ominaisuuksia seuraavasti:

**Työpöydän Outlook**

- Kohteen avaaminen
- Tiedosto -> Ominaisuudet -> Internet-otsikot

TAI

**Kävi koulua MFCMapi**

- Siirry Saapuneet-kansion kohteeseen
- Etsi PR_TRANSPORT_MESSAGE_HEADERS_W

Nämä ominaisuudet määritetään ja tallennetaan kuljetuksen ja reitityksen aikana. Lisävianmääritystä varten sinun on ehkä seurattava Kuljetustukea SPF:n, DKIM:n ja DMARC:n epäonnistumisista.