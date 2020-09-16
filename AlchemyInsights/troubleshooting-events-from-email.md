---
title: Tapahtumien vian määritys sähkö postista
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658731"
---
# <a name="troubleshooting-events-from-email"></a>Tapahtumien vian määritys sähkö postista

1. Tarkista, että ominaisuus on otettu käyttöön posti laatikolle: **Get-EventsFromEmailConfiguration <mailbox> -Identity**

2. Katso sitten tapahtumat sähkö postista-lokit **vienti-Mailposti-Diagnosticlogs <mailbox> -Component timeprofile**

3. Etsi tapahtumat Sähkö posti-lokista-kohdassa InternetMessageId, joka vastaa posti laatikon kohdetta.  

4. TrustScore määrittää, lisätäänkö kohde vai ei. Tapahtumia lisätään vain, jos Trustiscore = "luotettu".

TrustScore määräytyy SPF-, DKIM-tai dMarc-ominaisuuksien mukaan, jotka ovat viestin otsikossa.

Voit tarkastella näitä ominaisuuksia seuraavasti:

**Desktop Outlook**

- Kohteen avaaminen
- Tiedosto-> ominaisuudet-> Internet-otsikot

TAI

**Mfcmapia**

- Saapuneet-kansiossa olevaan kohteeseen siirtyminen
- Etsi PR_TRANSPORT_MESSAGE_HEADERS_W

Nämä ominaisuudet määritetään ja tallennetaan kuljetuksen ja reitityksen aikana. Jos haluat lisä tietoja vian määrityksestä, sinun on ehkä seurattava siirto tukea SPF-, DKIM-ja.-tai DMARC-virheiden varalta.