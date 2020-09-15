---
title: Outlookin Työpöytä version peruuttaminen tai sähkö posti viestin korvaaminen
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663987"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Outlook-Sähkö posti viestin peruuttaminen tai korvaaminen

- Järjestelmänvalvojana voit **peruuttaa viestejä käyttäjien puolesta PowerShellin avulla**. Et voi peruuttaa viestejä hallinta keskuksesta.
- Voit **peruuttaa vain organisaation henkilöille lähetetyt viestit**. Jos viesti on lähetetty Gmail-osoitteeseen, et voi esimerkiksi peruuttaa sitä.
- Voit **vain peruuttaa viestit, jotka on lähetetty Outlook 2016-tieto koneesta**. Jos käyttäjä lähettää viestin käyttämällä Outlook for Macia tai Outlookin verkko versiota, et voi peruuttaa sitä.

Sähkö posti viestin peruuttaminen tai korvaaminen:

1. Valitse Outlook-ikkunan vasemmalla puolella olevassa kansio ruudussa Lähetetyt-kansio.
1. Avaa viesti, jonka haluat peruuttaa, kaksoisnapsauttamalla sitä.
1. Valitse **viesti** -väli lehti ja valitse sitten **toiminnot**, jotka  >  **palauttavat tämän viestin**.
1. Valitse **Poista tämän viestin lukemattomat kopiot** tai **Poista lukemattomat kopiot ja vaihda uuteen viestiin**ja valitse sitten **OK**.
1. Jos lähetät korvaavan viestin, kirjoita viesti ja valitse sitten **Lähetä**.
1. Viestin peruuttamisen onnistuminen tai epäonnistuminen määräytyy sen mukaan, mitä vastaanottajia koskevat asetukset ovat Outlookissa. Jos haluat tarkistaa peruutuksen, Lue [Tämä artikkeli](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Sähkö posti viestien etsiminen ja poistaminen organisaatiossa

- Jos et ole yleinen järjestelmänvalvoja, tili on lisättävä eDiscoveryn hallinta rooliin tai yhteensopivuuden haun hallinta rooliin, jotta voit hakea viestejä. Jos haluat poistaa viestejä, sinun on liitytä organisaation hallinta-rooli ryhmään tai Hae ja poista hallinta-rooliin. Näiden roolien käyttö oikeudet määritetään [tieto turva-ja yhteensopivuus keskuksessa](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Luo sisältö haku](https://docs.microsoft.com/microsoft-365/compliance/content-search) , jos haluat etsiä poistettavan viestin.
- [Muodosta yhteys tieto turva-ja yhteensopivuus keskuksen PowerShellin avulla](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Jos käytät monimenetelmäistä todennusta, Katso lisä tietoja artikkelista [yhteyden muodostaminen Microsoft 365-tieto turva-ja yhteensopivuus keskuksen PowerShellin avulla monimenetelmäinen todentaminen-toiminnolla](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).