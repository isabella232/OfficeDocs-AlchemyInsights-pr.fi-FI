---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707908"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Korjaa virhekoodin 550 5.4.1 välityskäytön ongelmat estetty

Tämä ongelma [ilmenee, kun tarkistetaan, onko sähköpostiosoite kelvollinen estämään palautus,](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) kun siirryt Microsoft-verkkoon. Kokeile seuraavaa:

1. Selvitä, liittyykö ongelma koko toimialueeseen vai yhteen sähköpostiosoitteeseen:
    - Koko toimialue: Joskus toimialue on synkronoitava; yritä [asettaa toimialue sisäiseksi ja sitten takaisin arvovaltaiseen](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Yksittäinen sähköpostiosoite: Joskus osoite on synkronoitava; ailahteleminen smtp valtuutettu edustaja kohdistaa ja niin muodoin ailahteleminen se taaksepäin kanisteri auttaa.
2. Selvitä, liittyykö ongelma ryhmään vai yleiseen kansioon. Joissakin objektityypeissä objektit on ehkä luotava manuaalisesti Azure Active Directoryssa.

Jos tarvitset lisäapua, avaa tukipyyntö ja määritä ongelman laajuus (mukaan lukien lähetettävän objektin tyyppi), jotta voimme auttaa sinua paremmin.