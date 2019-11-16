---
title: AntiSpam 5.4.1 DBEB saalis-kaikki
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
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672430"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Korjaa toimitus ongelmat virhe koodissa 550 5.4.1 välityksen käyttö estetty

Tämä ongelma ilmenee, kun [tarkistetaan, onko Sähkö posti osoite kelvollinen estämään](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) käyttö ongelmia, kun siirrytään Office 365-verkkoon. Kokeile seuraavia:

1. Selvitä, onko ongelma koko toimi alueen vai yksittäisen Sähkö posti osoitteen osalta:
    - Koko verkko tunnus: joskus toimi alue on synkronoitava. Kokeile asettaa [toimi alueen sisäinen ja sitten takaisin arvovaltainen](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Yksittäinen Sähkö posti osoite: joskus osoite on synkronoitava; SMTP-välitys palvelimen osoitteen muuttaminen ja sen muuttaminen takaisin voi auttaa.
2. Selvitä, onko ongelma tiettyyn ryhmään vai yleiseen kansioon. Joidenkin objekti tyyppien kohdalla objektit on ehkä luotava manuaalisesti Azure Active Directoryssa.

Jos tarvitset lisä apua, avaa tuki pyyntö ja Määritä ongelman laajuus (includidng lähetävän objektin tyyppi), jotta voimme auttaa sinua paremmin.