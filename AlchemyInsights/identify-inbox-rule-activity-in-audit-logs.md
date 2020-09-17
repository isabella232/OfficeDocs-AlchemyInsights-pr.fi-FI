---
title: Saapuneet-kansion säännön aktiviteetin määrittäminen valvonta lokeissa
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779048"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Saapuneet-kansion säännön aktiviteetin määrittäminen valvonta lokeissa

Voit käyttää valvonta loki hakua Microsoft 365-tieto turva & yhteensopivuus keskuksessa, jos haluat tarkastella Saapuneet-kansion säännön tapahtumia (Saapuneet-kansion sääntöjen luominen, muokkaaminen ja poistaminen).

1. Kirjaudu sisään [Microsoft 365-tieto turva & Compliance Centeriin](https://protection.office.com/).

2. Siirry **haun**  >  **valvonta lokien haku** sivulle.

3. Valitse päivämäärä väli **alkamis päivä** -ja **päättymis päivä** -kenttiin.

4. Tarkista **Exchange-posti laatikon aktiviteetit**-kohdassa **aktiviteetit** -kentän arvoksi on valittu **New-inboxrule Luo/Muokkaa/Ota käyttöön tai Poista käytöstä Saapuneet-kansion sääntö**.

5. Valitse **Hae**.

Valitse tulokset-kohdassa valvonta tietue. Valitse tiedot-valikosta **lisä tietoja**. Tietoja Saapuneet-kansion säännön asetuksista näkyy **Parametrit** -kentässä.

Lisä tietoja on kohdassa [sen määrittäminen, onko käyttäjä luonut Saapuneet-kansion säännön](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
