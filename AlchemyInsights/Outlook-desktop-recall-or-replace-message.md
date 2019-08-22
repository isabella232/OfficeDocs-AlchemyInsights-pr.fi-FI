---
title: Työpöydän Outlook-peruutus- tai korvaa sähköpostiviestin
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496108"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Peruuttaa tai korvata Outlook-sähköpostiviesti

- Voit järjestelmänvalvojana, **peruutus viestien PowerShell avulla käyttäjien puolesta**. Ei voi peruuttaa viestien hallintakeskukseen.
- Voit **vain palauttaa viestit, jotka lähetetään organisaation henkilöt**. Jos viesti lähetettiin Gmail-osoite, esimerkiksi et pysty peruuttamaan sen.
- Voit **vain peruutus kulku Outlook-2016, PC: ssä**. Jos käyttäjä lähettää viestin käyttäen Mac Outlook tai Outlook Web, se ei voi peruuttaa.

Voit peruuttaa tai korvata sähköpostiviestin:

1. Valitse kansioruudusta Outlook-ikkunan vasemmassa reunassa Lähetetyt-kansioon.
1. Kaksoisnapsauta viestiä, jonka haluat peruuttaa, voit avata sen.
1. Valitse **sanoma** -välilehti ja valitse sitten **Toiminnot** > **Peruuta viesti**.
1. Valitse **poistaa viestin lukemattomat kopiot** tai **poistaa viestin lukemattomat kopiot ja korvata uudella viestillä**ja valitse sitten **OK**.
1. Jos lähetät korvaavan viestin, viestin, ja valitse sitten **Lähetä**.
1. Onnistuminen tai epäonnistuminen on viesti on riippuvainen vastaanottajan Outlook-asetuksista. Lisätietoja tarkistamisesta peruutus on [Tässä artikkelissa](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Etsi ja poista viestejä organisaation

- Jos et ole yleinen järjestelmänvalvoja, tili on lisättävä eDiscovery hallinnan rooli tai yhteensopivuuden haun hallinnan roolin voit hakea viestejä. Jos haluat poistaa viestejä, tarvitset liittyä organisaation hallinta-rooliryhmän tai etsintä- ja poisto-hallinnan roolin. Näiden roolien käyttöoikeuksista on liitetty [center tietoturvan ja määritystenmukaisuuden suhteen](https://go.microsoft.com/fwlink/?linkid=2083731).
- Voit etsiä poistettavan viestin [luominen on etsiä](https://docs.microsoft.com/office365/securitycompliance/content-search) .
- [Security and Compliance Centeriin PowerShell muodostaa](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Jos käytät monitasoisen todennuksen, katso [yhteyden Office 365: n tietoturvan ja yhteensopivuuden Center PowerShell monitasoisen todennuksen](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).