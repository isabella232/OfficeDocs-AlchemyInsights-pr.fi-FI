---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717358"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Virhe koodiin 550 5.4.1 Relay-käyttö estetty liittyvien ongelmien korjaaminen

Tämä ongelma ilmenee [, kun tarkistat, onko Sähkö posti osoite kelvollinen, jotta voit estää palautus viesteistä](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) , kun kirjoitat Microsoft Networkin. Kokeile seuraavaa:

1. Tarkista, koskeeko ongelma koko toimi aluetta vai yksittäistä Sähkö posti osoitetta:
    - Koko toimi alue: joskus toimi alue on synkronoitava. yritä [määrittää toimi alue sisäiseen käyttöön ja sitten takaisin arvovaltainen](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Yksittäinen Sähkö posti osoite: joskus osoite on synkronoitava; SMTP-välitys palvelimen osoitteen vaihtamiseen ja sen vaihtamiseen takaisin voi olla apua.
2. Määrittää, koskeeko ongelma tiettyä ryhmää vai julkista kansiota. Joidenkin objekti tyyppien objektit on ehkä luotava manuaalisesti Azure Active Directoryssa.

Jos tarvitset lisä ohjeita, voit avata tuki pyynnön ja määrittää ongelman laajuuden (mukaan lukien sen objektin tyypin, johon lähetät), jotta voimme auttaa sinua paremmin.