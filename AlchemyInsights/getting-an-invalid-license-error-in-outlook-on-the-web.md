---
title: 125 Saatko virheellisen käyttöoikeusvirheen Outlookin verkkoversio?
ms.author: daeite
author: daeite
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "125"
- "1600021"
ms.assetid: 6d9947d9-6c92-4ada-b655-8ab2a0c2b66d
ms.openlocfilehash: 357e57d20e3b6f56d3058bc1c782c3da7598520c29c5c29bfba6eec614fc5248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54089257"
---
# <a name="getting-an-invalid-license-error-in-outlook-on-the-web"></a>Saatko virheellisen käyttöoikeusvirheen Outlookin verkkoversio?

Jos käytät owa-Outlookin verkkoversio näyttöön tulee  Jotain meni vikaan -virhe, joka sisältää **X-OWA-Error-virheen: Microsoft.Exchange. Tiedot. Tallennus. InvalidLicenseException**, Exchange Online käyttöoikeus ei ole määritetty oikein tai se on äskettäin vanhentunut. Järjestelmänvalvoja voi määrittää käyttöoikeuden sinulle seuraavasti:
  
1. Avaa [Microsoft 365 -hallintakeskus](https://portal.office.com/adminportal/home#/homepage) **aktiiviset käyttäjät -kohdassa** **Muokkaa käyttäjää**.

2. Valitse **käyttäjä avautuu Muokkaa** käyttäjää -sivulla. Valitse käyttäjäominaisuuksien sivulla, joka avautuu, **Muokkaa** tuotteen **käyttöoikeuksia varten**.

3. Valitse tuotteen **käyttöoikeussivulla** sopiva Sijainti-arvo ja määritä käyttöoikeus, joka sisältää Exchange Online (laajenna käyttöoikeus, jotta näet sen tiedot).  Kun olet valmis, valitse **Tallenna**.
