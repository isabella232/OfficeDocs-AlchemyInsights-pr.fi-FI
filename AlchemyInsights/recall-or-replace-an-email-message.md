---
title: Sähkö posti viestin peruuttaminen tai korvaaminen
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353503"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Sähkö posti viestin peruuttaminen tai korvaaminen Microsoft 365-sovelluksessa

- Voit **peruuttaa vain organisaation henkilöille lähetetyt viestit**. Jos viesti on esimerkiksi lähetetty Gmail-osoitteeseen, et voi peruuttaa sitä.
- Voit **vain peruuttaa viestit, jotka on lähetetty Outlookista PC-tieto koneelle**. Jos käyttäjä lähettää viestin käyttämällä Outlook for Macia tai Outlookin verkko versiota, et voi peruuttaa sitä.
- Vuokra ajan järjestelmänvalvojana voit **peruuttaa viestit käyttäjien puolesta PowerShellin avulla** (lisä tietoja on artikkeleissa [Sähkö posti viestien etsiminen ja poistaminen](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Et voi peruuttaa viestejä hallinta keskuksesta. Lisä tietoja on kohdassa Sähkö posti viestien etsiminen ja poistaminen organisaatiossa.

**Lähetetyn Sähkö posti viestin peruuttaminen tai korvaaminen**

1. Valitse Outlook-ikkunan vasemmalla puolella olevassa kansio ruudussa Lähetetyt-kansio.
2. Avaa viesti, jonka haluat peruuttaa. Sinun on avattava viesti kaksoisnapsauttamalla. Kun valitset viestin niin, että se näkyy luku ruudussa, et voi peruuttaa viestiä.
3. Valitse viesti-väli lehdessä **toiminnot**, jotka  >  **palauttavat tämän viestin**.
4. Valitse **Poista viestin lukemattomat kopiot** tai **Poista lukemattomat kopiot ja vaihda uudella viestillä ja** valitse sitten **OK**.
5. Jos lähetät korvaavan viestin, kirjoita viesti ja valitse sitten **Lähetä**.
6. Viestin peruuttamisen onnistuminen tai epäonnistuminen määräytyy Outlookin edunsaajien asetusten mukaan.

Lisä tietoja, kuten peruutuksen tarkistaminen, on kohdassa [lähetetyn Sähkö posti viestin peruuttaminen tai korvaaminen](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Jos haluat **_etsiä ja poistaa organisaatiosi Sähkö posti viestejä_**, se on helpointa, jos olet yleinen järjestelmänvalvoja. Jos et ole yleinen järjestelmänvalvoja, tili on lisättävä eDiscoveryn hallinnan rooli ryhmään tai yhteensopivuuden haun hallinta rooliin. Jos haluat poistaa viestejä, sinun on liitytä organisaation hallinta-rooli ryhmään tai Hae ja poista hallinta-rooliin. Näiden roolien käyttö oikeudet määritetään [suojaus & yhteensopivuus keskuksessa](https://protection.office.com/).

1. [Luo sisältö haku](https://docs.microsoft.com/microsoft-365/compliance/content-search) , jos haluat etsiä poistettavan viestin.
2. [Muodosta yhteys tieto turva & Compliance Center PowerShellin avulla](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Jos käytössäsi on MFA (monimenetelmäinen todentaminen), Katso lisä tietoja artikkelista [yhteyden muodostaminen Microsoft 365-tieto turva & yhteensopivuus keskuksen PowerShell monimenetelmäisen todentamisen avulla](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
