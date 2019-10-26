---
title: Outlook Desktop muistaa tai korvata Sähkö posti viestin
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/25/2019
ms.locfileid: "36496108"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Outlook-Sähkö posti viestin peruuttaminen tai korvaaminen

- Järjestelmänvalvojana voit **peruuttaa viestit käyttäjien puolesta PowerShellin avulla**. Et voi peruuttaa viestejä hallinta keskuksesta.
- Voit **peruuttaa vain organisaatiosi henkilöille lähetetyt viestit**. Jos viesti lähetettiin esimerkiksi Gmail-osoitteeseen, et voi muistaa sitä.
- Voit **peruuttaa vain Outlook 2016-tieto koneella lähetetyt viestit**. Jos käyttäjä lähettää viestin Outlookin Mac-tai Outlook-tieto koneella, et voi muistaa sitä.

Sähkö posti viestin peruuttaminen tai korvaaminen:

1. Valitse Outlook-ikkunan vasemmalla puolella olevasta kansio ruudusta Lähetetyt-kansio.
1. Kaksoisnapsauta viestiä, jonka haluat peruuttaa, ja avaa se.
1. Valitse **viesti** -väli lehti ja valitse sitten **toiminnot** > **Muista tämä viesti**.
1. Valitse **Poista tämän viestin lukemattomat kopiot** tai **Poista lukemattomat kopiot ja korvaa ne uudella viestillä**ja valitse sitten **OK**.
1. Jos lähetät korvaavan viestin, kirjoita viesti ja valitse sitten **Lähetä**.
1. Viestin muistamisen onnistuminen tai epäonnistuminen riippuu vastaanottajan asetuksista Outlookissa. Lisä ohjeita takaisinkutsun tarkastamisen osalta [on tässä artikkelissa](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Etsi ja poista Sähkö posti viestejä organisaatiossasi

- Jos et ole yleinen järjestelmänvalvoja, sinun tilisi on lisättävä eDiscovery Managerin rooliin tai yhteensopivuuden haun hallinta rooliin, jotta voit etsiä viestejä. Jos haluat poistaa viestejä, sinun on liityttävä organisaation hallinta-rooli ryhmään tai haun ja Tyhjennen hallinnan rooliin. Näiden roolien käyttö oikeudet määritetään [Suojaus-ja yhteensopivuus keskuksessa](https://go.microsoft.com/fwlink/?linkid=2083731).
- Etsi poistettava viesti [luomalla sisältö haku](https://docs.microsoft.com/office365/securitycompliance/content-search) .
- [Muodosta yhteys tieto turva-ja yhteensopivuus keskukseen PowerShelliin](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Jos käytät monivaiheista todennusta, katso [yhteyden muodostaminen Office 365 Security and Compliance Center PowerShelliin monimivaiheisen todennuksen avulla](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).