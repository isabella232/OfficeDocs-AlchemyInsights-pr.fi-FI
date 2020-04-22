---
title: Saapuneet-kansion sääntöaktiviteetin tunnistaminen valvontalokeissa
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716421"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Saapuneet-kansion sääntöaktiviteetin tunnistaminen valvontalokeissa

Microsoft 365 Security & Compliance Centerin valvontalokihaun avulla voit tarkastella Saapuneet-kansion sääntötapahtumia (Saapuneet-kansion sääntöjen luominen, muokkaaminen ja poistaminen).

1. Kirjaudu Microsoft [365 Security & Compliance Centeriin.](https://protection.office.com/)

2. Siirry **Haun** > **valvontalokin hakusivulle.**

3. Valitse päivämääräväli **Aloituspäivä-** ja **Päättymispäivä-kentissä.**

4. Tarkista **Exchange-postilaatikkoaktiviteetit**-kohdassa, että **Aktiviteetit-kentän** arvoksi on määritetty **Uusi Saapuneet-kansion sääntö Luo/muokkaa/ota käyttöön tai poista käytöstä .**

5. Valitse **Hae**.

Valitse tuloksista valvontatietue. Valitse tiedot-pikaikkunassa **Lisätietoja**. Saapuneet-kansion säännön asetusten tiedot näkyvät **Parametrit-kentässä.**

Lisätietoja on [ohjeaiheessa Sen määrittäminen, onko käyttäjä luonut Saapuneet-kansion säännön](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
