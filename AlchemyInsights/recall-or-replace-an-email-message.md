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
ms.openlocfilehash: e958dab159e4dcc11f9c068bded3aa06ccd65c15
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509453"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Sähköpostiviestin peruuttaminen tai korvaaminen Microsoft 365:ssä

- Voit **palauttaa vain organisaation henkilöille lähetetyt viestit.** Jos viesti on lähetetty esimerkiksi Gmail-osoitteeseen, et muista sitä.
- Voit **peruuttaa vain Outlook 2016:sta pc:lle lähetetyt viestit.** Jos käyttäjä lähettää viestin Outlook for Macilla tai Outlookin verkkoversiossa, et muista sitä.
- Jos olet järjestelmänvalvoja, voit **palauttaa viestit käyttäjien puolesta PowerShellin avulla.** Et voi palauttaa viestejä hallintakeskuksesta. Saat lisätietoja vierittämällä alaspäin kohtaan Etsi ja poista sähköpostiviestejä organisaatiostasi.

**Lähettämäsi sähköpostiviestin peruuttaminen tai korvaaminen**

1. Valitse Outlook-ikkunan vasemmalla puolella olevasta kansioruudusta Lähetetyt-kansio.
2. Avaa viesti, jonka haluat palauttaa. Avaa viesti kaksoisnapsauttamalla sitä. Viestin valitseminen siten, että se näkyy lukuruudussa, et voi palauttaa viestiä.
3. Valitse Viesti-välilehdessä **Actions**  >  **Toiminnot, jotka palauttavat tämän viestin**.
4. Valitse **Poista tämän viestin lukemattomat kopiot** tai Poista **lukemattomat kopiot ja korvaa se uudella viestillä**ja valitse sitten **OK**.
5. Jos lähetät korvaavan viestin, kirjoita viesti ja valitse sitten **Lähetä**.
6. Viestin palauttamisen onnistuminen tai epäonnistuminen riippuu vastaanottajien outlookin asetuksista.

Lisätietoja, kuten palautustietojen tarkistamisesta, on ohjeaiheessa [Lähettämäsi sähköpostiviestin peruuttaminen tai korvaaminen](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Sähköpostiviestien etsiminen ja poistaminen organisaatiossa*** Jos haluat etsiä ja poistaa sähköpostiviestejä organisaatiostasi, on helpointa, jos olet yleinen järjestelmänvalvoja. Jos et ole yleinen järjestelmänvalvoja, tilisi on lisättävä eDiscovery Manager -rooliryhmään tai Yhteensopivuushaun hallintarooliin. Jos haluat poistaa viestejä, sinun on liityttävä Organisaation hallinta -rooliryhmään tai Haun ja Tyhjennä -hallintarooliin. Näiden roolien käyttöoikeudet määritetään [Suojaus & -yhteensopivuuskeskuksessa.](https://protection.office.com/)

1. Etsi poistettava viesti [luomalla sisältöhaku.](https://docs.microsoft.com/microsoft-365/compliance/content-search)
2. [Muodosta yhteys & Compliance Center PowerShell -palveluun.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps) 

Jos käytät MFA:ta, katso [lisätietoja ohjeaiheesta Yhteyden muodostaminen Microsoft 365 security & Compliance Center PowerShelliin monivaiheisen todennuksen avulla](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
