---
title: 618 Kalenterin jakamiskäytäntö
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/26/2020
ms.locfileid: "44372996"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Käytäntövirhe kalenteria jaettaessa

1. Tee jokin seuraavista tilanteesi mukaan:
    - Muodosta yhteys Exchange Onlineen PowerShellin etäyhteyden avulla. Lisätietoja on ohjeaiheessa [Yhteyden muodostaminen Exchange Onlineen PowerShellin etäyhteyden avulla](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Avaa exchange-hallintaliittymä paikallisessa palvelimessa.
2. Määritä käyttäjälle määritetty jakamiskäytäntö. Voit tehdä tämän suorittamalla seuraavan komennon ja merkitsemään muistiin käytännön palautetun komennon:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Päivitä käyttäjän jakamiskäytäntö. Voit tehdä tämän seuraavasti:
    - Avaa Exchange-hallintakeskus.
    - Valitse **Organisaatio**ja kaksoisnapsauta sitten käyttäjälle määritettyä käytäntöä **Kohdassa Yksilöllinen jakaminen**. Tämä käytäntö palautettiin vaiheessa 2.
    - Valitse Jakamissääntö-sivun **Määritä jaettavat tiedot**-kohdasta kalenterin jakamistaso. valitse **Tallenna**.

Lisätietoja on [ohjeaiheessa Käytäntö ei salli käyttöoikeuksien myöntämistä yhdelle tai useammalle vastaanottajalle -virhe, kun käyttäjä yrittää jakaa kalenteria](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
