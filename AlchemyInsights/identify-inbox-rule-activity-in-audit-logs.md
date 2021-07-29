---
title: Saapuneet-kansion säännön toiminnan tunnistaminen valvontalokeja varten
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
ms.openlocfilehash: 3bda32b55be9c2fa671376e73b06aadfbe976363
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630174"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Saapuneet-kansion säännön toiminnan tunnistaminen valvontalokeja varten

Voit tarkastella Saapuneet-kansion sääntöjen tapahtumia Microsoft 365-& valvontalokihaun avulla (Saapuneet-kansion sääntöjen luominen, muokkaaminen ja poistaminen).

1. Kirjaudu Microsoft 365 [yhteensopivuuskeskukseen.](https://protection.office.com/)

2. Siirry haun   >  **valvontalokihakusivulle.**

3. Valitse päivämääräalue Alkamispäivä- ja **Päättymispäivä-kentistä.** 

4. Tarkista **Exchange Postilaatikon** toiminnot -kohdassa, että Toiminnot-kentän arvoksi on määritetty **Uusi Saapuneet-kansioRule Luo, muokkaa/ota käyttöön tai poista käytöstä Saapuneet-kansion sääntö.** 

5. Valitse **Hae**.

Valitse tuloksista valvontatietue. Valitse tiedot-pikaikkunassa **Lisätietoja**. Tiedot Saapuneet-kansion sääntöasetuksista näkyvät **Parametrit-kentässä.**

Lisätietoja on kohdassa Käyttäjän [Saapuneet-kansion säännön luomisen selvittäminen](/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
