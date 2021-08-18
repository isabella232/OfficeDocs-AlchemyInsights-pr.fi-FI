---
title: Viestien poistotapahtumien tunnistaminen valvontalokeissa
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f5d6041fd80b4d5cae610e7d9248e45ed410a3d9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317591"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Poistettujen sähköpostiviestien valvontalokit

Tammikuusta 2019 alkaen Microsoft on ottanut postilaatikoiden valvontalokit oletusarvoisesti käyttöön. Jos haluat tarkastella tietyn käyttäjän viestien poistotapahtumia, sinun on otettava valvontatoiminnot käyttöön manuaalisesti. Jos postilaatikon valvontaloki on jo käytössä organisaatiossasi tai tietyllä käyttäjällä, noudata seuraavia ohjeita.

1. Kirjaudu Microsoft 365 [yhteensopivuuskeskukseen](https://protection.office.com/)

2. Valitse **Haku ja tutkimus** ja valitse **Valvontalokihaku**.

3. Valitse päivämääräalue Alkamispäivä- ja **Päättymispäivä-kentistä.**  Määritä sen käyttäjän käyttäjänimi, jonka haluat tutkia (kohteiden poistanut käyttäjä). Valitse **Toiminnot-kentässä** **Poistetut viestit Poistetut-kansiosta ja** **Siirretty viestit Poistetut-kansioon**.

4. Valitse **Hae**.

Valitse tuloksista valvontatietue. Valitse tiedot-pikaikkunassa **Lisätietoja**. Lisätietoja poistetusta kohteesta (esimerkiksi aiherivi ja kohteen sijainti, kun se poistettiin) näytetään **AffectedItems-kentässä.** **ClientInfoString-ominaisuus** näyttää, jos poisto on tapahtunut Outlook-, Outlookin verkkoversio (aiemmin Outlook Web App) tai missä tahansa muissa laitteessa.

Lisätietoja on kohdassa [Postilaatikon sähköpostin edelleenlähetysten määritysten selvittäminen.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Huomautus:** Poistettuja kohteita ei voi noutaa valvontalokitoiminnolla. Lisätietoja poistettujen viestien Outlookin verkkoversio on kohdassa [Poistettujen kohteiden palauttaminen Outlook Web App.](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)
