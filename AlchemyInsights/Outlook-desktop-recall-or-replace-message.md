---
title: Outlook Sähköpostiviestin takaisinveto tai korvaaminen työpöydällä
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
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918392"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Sähköpostiviestin Outlook tai korvaaminen

- Järjestelmänvalvojana voit peruuttaa **viestejä käyttäjien puolesta PowerShellin avulla.** Et voi peruuttaa viestejä hallintakeskuksesta.
- Voit peruuttaa **vain viestit, jotka on lähetetty organisaatiosi käyttäjille.** Jos viesti on lähetetty esimerkiksi Gmail-osoitteeseen, et voi peruuttaa sitä.
- Voit peruuttaa **vain tietokoneesta Outlook 2016 lähetetyt viestit.** Jos käyttäjä lähettää viestin käyttämällä Outlook for Mac tai Outlookin verkkoversio, et voi peruuttaa sitä.

Sähköpostiviestin peruutaminen tai korvaaminen:

1. Valitse Lähetetyt-kansio kansioruudussa Outlook ikkunan vasemmalla puolella.
1. Avaa viesti kaksoisnapsauttamalla viestiä, jonka haluat peruuttaa.
1. Valitse **Viesti-välilehti** ja valitse sitten   >  **Toiminnot, jotka peruutavat tämän viestin**.
1. Valitse **Poista viestin lukemattomat kopiot tai** Poista lukemattomat kopiot ja korvaa **uudella viestillä** ja valitse sitten **OK**.
1. Jos lähetät korvaavan viestin, kirjoita viesti ja valitse sitten **Lähetä**.
1. Viestin takaisinkutsun onnistuminen tai epäonnistuminen riippuu vastaanottajan asetuksista viestin Outlook. Lisätietoja muistamisen tarkistamisen vaiheista on [tässä artikkelissa.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

Sähköpostiviestien etsiminen ja poistaminen organisaatiossa

- Jos et ole yleinen järjestelmänvalvoja, tili on lisättävä eDiscovery Manager -rooliin tai yhteensopivuushaun hallintarooliin viestien hakemista varten. Jos haluat poistaa viestejä, sinun täytyy liittyä Organisaation hallinta -rooliryhmään tai Haku- ja poisto-hallintarooliin. Näiden roolien käyttöoikeudet määritetään tietoturva- [ja yhteensopivuuskeskuksessa.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [Etsi poistettava viesti](https://docs.microsoft.com/microsoft-365/compliance/content-search) luomalla sisältöhaku.
- [Näyttöyhteys tietoturva- ja yhteensopivuuskeskuksen PowerShelliin.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Jos käytät monimenetelmäistä todentamista, katso lisätietoja Näyttöyhteys Microsoft 365 ja [yhteensopivuuskeskuksen PowerShellin käyttämisestä monimenetelmäisen todentamisen avulla.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)