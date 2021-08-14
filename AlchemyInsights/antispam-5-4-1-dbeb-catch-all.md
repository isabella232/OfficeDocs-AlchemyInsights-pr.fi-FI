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
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932274"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Korjaa toimitusongelmat virhekoodille 550 5.4.1 Välityksen käyttö estetty

Tämä ongelma ilmenee, [kun tarkistetaan, onko](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) sähköpostiosoite kelvollinen, jotta se ei pääse siirtymään Microsoft-verkkoon. Kokeile seuraavaa:

1. Määritä, onko ongelma erityinen koko toimialueelle vai yksittäiselle sähköpostiosoitteelle:
    - Koko toimialue: Joskus toimialue on synkronoitava. kokeile [määrittää toimialueeksi Sisäinen ja sitten takaisin Päätoimialue.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - Yksittäinen sähköpostiosoite: Joskus osoite on synkronoitava. SMTP-välityspalvelimen osoitteen muuttaminen ja sen muuttaminen takaisin voi auttaa.
2. Määritä, onko ongelma ryhmässä vai julkisessa kansiossa. Jotkin objektityypit on ehkä luotava manuaalisesti Azure Active Directory.

Jos tarvitset lisätukea, avaa tukipalvelupyynnön ja määritä ongelman laajuus (mukaan lukien sen objektin tyyppi, jolle lähetät), jotta voimme auttaa sinua paremmin.