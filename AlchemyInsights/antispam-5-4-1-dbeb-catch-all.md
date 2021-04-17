---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821444"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Korjaa toimitusongelmat virhekoodille 550 5.4.1 Välityksen käyttö estetty

Tämä ongelma ilmenee, [kun tarkistetaan, onko](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) sähköpostiosoite kelvollinen, jotta se ei pääse siirtymään Microsoft-verkkoon. Kokeile seuraavaa:

1. Määritä, onko ongelma erityinen koko toimialueelle vai yksittäiselle sähköpostiosoitteelle:
    - Koko toimialue: Joskus toimialue on synkronoitava. kokeile [määrittää toimialueeksi Sisäinen ja sitten takaisin Päätoimialue.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - Yksittäinen sähköpostiosoite: Joskus osoite on synkronoitava. SMTP-välityspalvelimen osoitteen muuttaminen ja sen muuttaminen takaisin voi auttaa.
2. Määritä, onko ongelma ryhmässä vai julkisessa kansiossa. Jotkin objektityypit on ehkä luotava manuaalisesti Azure Active Directoryssa.

Jos tarvitset lisätukea, avaa tukipalvelupyynnön ja määritä ongelman laajuus (mukaan lukien sen objektin tyyppi, jolle lähetät), jotta voimme auttaa sinua paremmin.