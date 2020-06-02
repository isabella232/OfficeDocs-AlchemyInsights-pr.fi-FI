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
ms.openlocfilehash: bb84363ae7d3c91750d5de789c091c7cebbbedc2
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502316"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Outlook-sähköpostiviestin peruuttaminen tai korvaaminen

- Järjestelmänvalvojana voit **palauttaa viestit käyttäjien puolesta PowerShellin avulla.** Et voi palauttaa viestejä hallintakeskuksesta.
- Voit **palauttaa vain organisaation henkilöille lähetetyt viestit.** Jos viesti on lähetetty esimerkiksi Gmail-osoitteeseen, et muista sitä.
- Voit **palauttaa outlook 2016:sta lähetetyt viestit vain tietokoneessa**. Jos käyttäjä lähettää viestin Outlook for Macilla tai Outlookin verkkoversiossa, et muista sitä.

Sähköpostiviestin peruuttaminen tai korvaaminen:

1. Valitse Outlook-ikkunan vasemmalla puolella olevasta kansioruudusta Lähetetyt-kansio.
1. Avaa se kaksoisnapsauttamalla viestiä, jonka haluat palauttaa.
1. Valitse **Viesti-välilehti** ja valitse sitten **Toiminnot**  >  **peruuta tämä viesti**.
1. Valitse **Poista tämän viestin lukemattomat kopiot** tai Poista **lukemattomat kopiot ja korvaa se uudella viestillä**ja valitse sitten **OK**.
1. Jos lähetät korvaavan viestin, kirjoita viesti ja valitse sitten **Lähetä**.
1. Viestin palauttamisen onnistuminen tai epäonnistuminen riippuu vastaanottajan outlookin asetuksista. Lisätietoja palautusten tarkistamisesta on [tässä artikkelissa](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Sähköpostiviestien etsiminen ja poistaminen organisaatiossa

- Jos et ole yleinen järjestelmänvalvoja, tilisi on lisättävä eDiscovery Manager -rooliin tai yhteensopivuushaun hallintarooliin, jotta voit etsiä viestejä. Jos haluat poistaa viestejä, sinun on liityttävä Organisaation hallinta -rooliryhmään tai Haun ja Tyhjennä -hallintarooliin. Näiden roolien käyttöoikeudet määritetään [Suojaus- ja yhteensopivuuskeskuksessa.](https://go.microsoft.com/fwlink/?linkid=2083731)
- Etsi poistettava viesti [luomalla sisältöhaku.](https://docs.microsoft.com/microsoft-365/compliance/content-search)
- [Muodosta yhteys Tietoturva- ja Compliance Center PowerShell -sovellukseen.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Jos käytät monivaiheista todennusta, katso [lisätietoja ohjeaiheesta Yhteyden muodostaminen Microsoft 365 :n tietoturvaan ja Compliance Center PowerShelliin monivaiheisen todennuksen avulla](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).