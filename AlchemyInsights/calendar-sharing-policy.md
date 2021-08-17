---
title: 618 Kalenterin jakamiskäytäntö
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091600"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Käytäntövirhe kalenteria jaettaessa

1. Tee tilanteesi mukaan jokin seuraavista:
    - Näyttöyhteys Exchange Online PowerShellin avulla. Lisätietoja on kohdassa [PowerShell-Näyttöyhteys Exchange Online käyttäminen.](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)
    - Avaa paikallisessa palvelimessa Exchange hallintaliittymä.
2. Määritä käyttäjälle määritetty jakamiskäytäntö. Voit tehdä tämän seuraavalla komennolla ja panemalla muistiin palautetun käytännön:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Päivitä käyttäjän jakamiskäytäntö. Voit tehdä tämän seuraavasti:
    - Avaa Exchange hallintakeskus.
    - Valitse **Organisaatio** ja kaksoisnapsauta sitten käytäntöä, joka on määritetty käyttäjälle Kohdassa **Yksittäinen jakaminen**. Tämä on käytäntö, joka palautettiin vaiheessa 2.
    - Valitse Jakamissääntö-sivulla kalenterin jakamistaso, jonka haluat sallia kohdassa **Määritä, mitkä** tiedot haluat jakaa ; Valitse **Tallenna.**

Lisätietoja on seuraavassa ohjeaiheessa: "Käytäntö ei salli käyttöoikeuksien myöntämistä tällä tasolla yhdelle tai yhdelle tai yhdelle vastaanottajalle" -virhe, kun käyttäjä yrittää [jakaa kalenterin.](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)
