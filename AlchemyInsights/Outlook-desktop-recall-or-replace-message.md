---
title: Outlook Desktopin sähköpostiviestin peruuttaminen tai korvaaminen
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: d64332778f9132aff6a9660bb0d522f4e16b753c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687507"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Outlook-sähköpostiviestin peruuttaminen tai korvaaminen

- Järjestelmänvalvojana voit **palauttaa viestit PowerShelliä käyttävien käyttäjien puolesta.** Et voi palauttaa viestejä hallintakeskuksesta.
- Voit **vain muistaa viestejä, jotka lähetetään organisaatiosi henkilöille.** Jos viesti on esimerkiksi lähetetty Gmail-osoitteeseen, et voi muistaa sitä.
- Voit **vain palauttaa Outlook 2016:sta lähetetyt viestit tietokoneeseen**. Jos käyttäjä lähettää viestin Outlook for Macin tai Outlookin verkkoversiossa, et voi muistaa sitä.

Sähköpostiviestin peruuttaminen tai korvaaminen:

1. Valitse Outlook-ikkunan vasemmalla puolella olevasta kansioruudusta Lähetetyt-kansio.
1. Avaa se kaksoisnapsauttamalla viestiä, jonka haluat palauttaa.
1. Valitse **Viesti-välilehti** ja valitse sitten **Toiminnot, jotka** > **poistavat tämän viestin**.
1. Valitse **Poista tämän viestin lukemattomat kopiot** tai Poista **lukemattomat kopiot ja korvaa se uudella viestillä**ja valitse sitten **OK**.
1. Jos lähetät korvaavan viestin, kirjoita viesti ja valitse sitten **Lähetä**.
1. Viestin peruuttaminen riippuu vastaanottajan outlook-asetuksista. Ohjeet palautuksen tarkistamiseen ovat [tässä artikkelissa](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Sähköpostiviestien etsiminen ja poistaminen organisaatiossa

- Jos et ole yleinen järjestelmänvalvoja, tilisi on lisättävä eDiscovery Manager -rooliin tai Yhteensopivuushaun hallintarooliin viestien etsimistä varten. Jos haluat poistaa viestejä, sinun on liityttävä Organisaation hallinta -rooliryhmään tai Haku- ja Tyhjennyshallinta-rooliin. Näiden roolien käyttöoikeudet määritetään [Suojaus- ja yhteensopivuuskeskuksessa](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Luo sisältöhaku,](https://docs.microsoft.com/office365/securitycompliance/content-search) jotta voit etsiä poistettavan viestin.
- [Muodosta yhteys Suojaus- ja Yhteensopivuuskeskus PowerShelliin](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Jos käytät monivaiheista todennusta, katso [yhteyden muodostaminen Microsoft 365 :n suojaus- ja Yhteensopivuuskeskus PowerShelliin monivaiheisen todennuksen avulla](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).