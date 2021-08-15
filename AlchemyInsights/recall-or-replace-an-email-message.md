---
title: Sähköpostiviestin peruutaminen tai korvaaminen
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
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024383"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Sähköpostiviestin peruutaminen tai korvaaminen Microsoft 365

- Voit peruuttaa **vain viestit, jotka on lähetetty organisaatiosi käyttäjille.** Jos viesti on esimerkiksi lähetetty Gmail-osoitteeseen, et voi peruuttaa sitä.
- Voit peruuttaa **vain viestit, jotka on lähetetty Outlook tietokoneesta**. Jos käyttäjä lähettää viestin käyttämällä Outlook for Mac tai Outlookin verkkoversio, et voi peruuttaa sitä.
- Vuokraajan järjestelmänvalvojana voit peruuttaa viestejä käyttäjien puolesta **PowerShellin** avulla (Lisätietoja on ohjeaiheessa Sähköpostiviestien etsiminen [ja poistaminen).](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)
- Et voi peruuttaa viestejä hallintakeskuksesta. Vieritä alaspäin kohtaan "Hae ja poista sähköpostiviestejä organisaatiossasi", niin saat lisätietoja.

**Lähetetyn sähköpostiviestin peruutaminen tai korvaaminen**

1. Valitse kansioruudussa, joka on Outlook-ikkunan vasemmalla puolella, ja valitse Lähetetyt-kansio.
2. Avaa viesti, jonka haluat peruuttaa. Avaa viesti kaksoisnapsauttamalla. Jos valitset viestin siten, että se näkyy lukuruudussa, et voi peruuttaa viestiä.
3. Valitse Viesti-välilehdessä **Toiminnot Peruuta** tämä  >  **viesti**.
4. Valitse **Poista viestin lukemattomat kopiot tai** Poista lukemattomat kopiot ja korvaa **uudella viestillä** ja valitse sitten **OK**.
5. Jos lähetät korvaavan viestin, kirjoita viesti ja valitse sitten **Lähetä**.
6. Viestin takaisinkutsun onnistuminen tai epäonnistuminen riippuu vastaanottajan asetuksista Outlook.

Lisätietoja, kuten ohjeet viestin muistamisen tarkistamisen tarkistamaan, on kohdassa Lähettämäsi [sähköpostiviestin peruutaminen tai korvaaminen.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

***Sähköpostiviestien etsiminen ja poistaminen organisaatiossa*** on helpointa, jos olet yleinen järjestelmänvalvoja. Jos et ole yleinen järjestelmänvalvoja, tilisi on lisättävä eDiscovery Manager -rooliryhmään tai yhteensopivuushaun hallintarooliin. Jos haluat poistaa viestejä, sinun täytyy liittyä Organisaation hallinta -rooliryhmään tai Haku- ja poisto-hallintarooliin. Näiden roolien käyttöoikeudet määritetään tietoturva- & [yhteensopivuuskeskuksessa.](https://protection.office.com/)

1. [Etsi poistettava viesti](https://docs.microsoft.com/microsoft-365/compliance/content-search) luomalla sisältöhaku.
2. [Näyttöyhteys tietoturva- & PowerShelliin.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)

Jos käytössäsi on monimenetelmäinen todentamismenetelmä, tutustu Näyttöyhteys Microsoft 365:& PowerShellin tietoturva- ja yhteensopivuuskeskuksen [PowerShellin monimenetelmäisen todentamisen avulla.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
