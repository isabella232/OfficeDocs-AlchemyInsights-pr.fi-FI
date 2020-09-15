---
title: 618-kalenterin jakamis käytännöt
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
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684227"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Käytäntöä koskeva virhe kalenteria jaettaessa

1. Tee tilan teen mukaan jokin seuraavista:
    - Muodosta yhteys Exchange Onlineen PowerShell-etätoiminnolla. Lisä tietoja on Ohje aiheessa [yhteyden muodostaminen Exchange Onlineen PowerShellin etätoiminnolla](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Avaa Exchange-hallinta liittymä paikallisessa palvelimessa.
2. Määrittää käyttäjälle määritetyn jakamis käytäntöjen. Jos haluat tehdä tämän, suorita seuraava komento ja huomioi sen palauttama menettely:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Päivitä käyttäjän jakamis käytäntöä. Voit tehdä tämän seuraavasti:
    - Avaa Exchange-hallinta keskus.
    - Valitse **organisaatio**ja kaksoisnapsauta sitten **yksittäistä jakoa**varten määritettyä käytäntöä. Tämä on vaiheessa 2 palautettu käytännöt.
    - Valitse jakamis sääntö-sivulla sen kalenterin jakamis taso, jonka haluat sallia, kohdassa Määritä, **mitä tietoja haluat jakaa**. Valitse **Tallenna**.

Lisä tietoja on kohdassa ["käytännöt eivät salli oikeuksien myöntämistä tällä tasolla yhdelle tai useammalle vastaanottajalle"-virhe, kun käyttäjä yrittää jakaa kalenteria](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
