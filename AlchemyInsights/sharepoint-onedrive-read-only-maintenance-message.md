---
title: Vain luku-ylläpito tulee näyttöön, kun yrität käyttää SharePoint- tai OneDrive
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620720"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Vain luku-ylläpito tulee näyttöön, kun yrität käyttää SharePoint- tai OneDrive

Käyttäjät saattavat saada **Ylläpito vain luku -** viestin, kun yrität käyttää SharePoint- tai OneDrive seuraavissa tilanteissa. 

-   Suunniteltu tai aktiivinen huoltotoimet.  Tarkista ne siirtymällä [Message Center](https://portal.office.com/adminportal/home#/messagecenter).
-   Suuren prioriteetin aktiivisen palvelun ajankohta, joka on esiintyvä. Tarkista siirtymällä [Terveyden huollon](https://portal.office.com/adminportal/home#/servicehealth)tiedotteiden ja tapahtumat.
-   Pieni auto kenties recovery skenaario, joka saattaa toimi koska odottamattomia tapahtumia palvelimissa, jotka saattavat kestää alle 30 minuuttia tai niin. 
    
    On Message Center ei ole tai palvelu terveyden kirjaa nämä pienet saantotiedot mutta pitäisi olla takaisin normaaliksi on hyvin pian.

Vain muutamia kertoja olemme havaitaan jokin edellä mainitut kolme tilanteita on ollut syy, ja palvelu on palautettu mutta käyttäjien selaimen välimuisti ei ole vielä tyhjennetty.

Yritä tyhjentää selaimen välimuisti ennen sivuston navigointi.

1. Microsoft Edge-selaimessa Valitse **asetukset**ja valitse sitten **Tietosuoja- ja**.
2. Valitse **Poista selaaminen**, **Valitse mitä haluat poistaa**.
3. **Evästeet ja tallennetun Web-sivun tiedot**ja valitse **Poista**.

>[!Note] 
> Nämä vaiheet saattavat vaihdella muissa selaimissa, kuten Mozilla Firefox tai Google Chrome.

>[!Note] 
> Avaa uusi InPrivate-ikkunassa SharePoint-sivuston tai OneDrive olisi toinen vaihtoehto.