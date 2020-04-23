---
title: Sähköpostiviestin peruuttaminen tai korvaaminen
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e541620a499b02a7206579ffcc505ceb4e632a4c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742752"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Sähköpostiviestin peruuttaminen tai korvaaminen Microsoft 365:ssä

- Voit **vain muistaa viestejä, jotka lähetetään organisaatiosi henkilöille.** Jos viesti on esimerkiksi lähetetty Gmail-osoitteeseen, et voi muistaa sitä.
- Voit **palauttaa vain Outlook 2016:sta pc:lle lähetetyt viestit.** Jos käyttäjä lähettää viestin Outlook for Macin tai Outlookin verkkoversiossa, et voi muistaa sitä.
- Jos olet järjestelmänvalvoja, voit **palauttaa viestit käyttäjien puolesta PowerShellin avulla.** Et voi palauttaa viestejä hallintakeskuksesta. Saat lisätietoja vierittämällä alaspäin kohtaan Etsi ja poista sähköpostiviestejä organisaatiossasi.

**Lähettämäsi sähköpostiviestin peruuttaminen tai korvaaminen**

1. Valitse Outlook-ikkunan vasemmalla puolella olevasta kansioruudusta Lähetetyt-kansio.
2. Avaa viesti, jonka haluat palauttaa. Sinun on avattava viesti kaksoisnapsauttamalla. Kun valitset viestin siten, että se näkyy lukuruudussa, et voi palauttaa viestiä.
3. Valitse Viesti-välilehdessä **Toiminnot, jotka** > **poistavat tämän viestin**.
4. Valitse **Poista tämän viestin lukemattomat kopiot** tai Poista **lukemattomat kopiot ja korvaa se uudella viestillä**ja valitse sitten **OK**.
5. Jos lähetät korvaavan viestin, kirjoita viesti ja valitse sitten **Lähetä**.
6. Viestin peruuttaminen riippuu vastaanottajien outlook-asetuksista.

Lisätietoja, kuten palautusilmoituksen tarkistaminen, on ohjeaiheessa [Lähettämäsi sähköpostiviestin peruuttaminen tai korvaaminen](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Sähköpostiviestien etsiminen ja poistaminen organisaatiossa*** Jos haluat etsiä ja poistaa sähköpostiviestejä organisaatiossasi, on helpointa, jos olet yleinen järjestelmänvalvoja. Jos et ole yleinen järjestelmänvalvoja, tilisi on lisättävä eDiscovery Manager -rooliryhmään tai Yhteensopivuushaun hallintarooliin. Jos haluat poistaa viestejä, sinun on liityttävä Organisaation hallinta -rooliryhmään tai Haku- ja Tyhjennyshallinta-rooliin. Näiden roolien käyttöoikeudet määritetään [Suojaus-& yhteensopivuuskeskuksessa](https://protection.office.com/).

1. [Luo sisältöhaku,](https://docs.microsoft.com/office365/securitycompliance/content-search) jotta voit etsiä poistettavan viestin.
2. [Muodosta yhteys Security & Compliance Center PowerShelliin.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps) 

Jos käytät MFA:ta, katso [yhteyden muodostaminen Microsoft 365:n tietoturva& Compliance Center PowerShelliin monivaiheisen todennuksen avulla](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
