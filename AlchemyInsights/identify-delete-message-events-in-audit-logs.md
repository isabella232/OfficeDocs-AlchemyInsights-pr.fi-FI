---
title: Seurantalokien poistaminen viestin tapahtumien selvittäminen
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32416707"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Postitettujen viestien valvontalokissa.

Tammikuuta 2019 alkaen Microsoft on ottaminen käyttöön postilaatikon valvonta on oletusarvon mukaan kirjaaminen. Muussa tapauksessa poista viesti tapahtumia tietyn käyttäjän tarkastelemaan täytyy ottaa käyttöön manuaalisesti Poista toimintojen valvonta Jos postilaatikon valvonnan kirjaaminen on jo käytössä organisaation tai tietyn käyttäjän, alla olevien ohjeiden mukaisesti.

1. Kirjautua [Office 365-suojauksen & Compliance Centeriin](https://protection.office.com/)

2. **Etsi ja tutkimus** ja valitse **Valvo lokista etsintää**.

3. Valitse **aloituspäivä** - ja **päättymispäivä** -kenttiin päivämääräalue. Määritä käyttäjänimi käyttäjä, jonka haluat tutkia (käyttäjä joka poistaa nimikkeitä). Valitse **aktiviteetit** -kentässä **Poistetut viestit Poistetut-kansiosta** ja **Moved viestit Poistetut-kansioon**.

4. Valitse **Etsi**.

Valitse tulosten koskeva seurantatietue. Valitse tiedot-valikon avauspainike **Lisätietoja**. **AffectedItems** -kentässä näkyy lisätietoja poistetun kohteen (esimerkiksi aihe ja sijainti kohde, kun se on poistettu). **ClientInfoString** -ominaisuus näyttää, jos Outlookissa, Outlook web (tunnettiin aiemmin nimellä Outlook Web App), tai muussa laitteessa tapahtunut poisto.

Lisätietoja [määrittäminen, joka määrittää sähköpostiviestin välittäminen postilaatikkoon](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Huomautus**: audit log-toiminnolla poistettuja kohteita ei voi noutaa. Noutamaan poistetut viestit Outlook Web-kohdassa [Palauta poistetut viestit Outlook Web Appissa](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
