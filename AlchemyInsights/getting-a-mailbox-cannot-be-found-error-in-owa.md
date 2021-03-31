---
title: 126 Postilaatikon saaminen ei löydy virheestä OWA:ssa?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426659"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Saatko postilaatikon, joka ei löydy -virheestä Outlookin verkkosovelluksessa?

Jos käytät Outlookin verkkotiliä ja  saat virheilmoituksen postilaatikosta, tiliä, jolla muodostat yhteyden Outlookin verkkosovellukseen, ei ole Exchange Online -käyttöoikeutta, joten tiliin ei ole liitetty postilaatikkoa. Järjestelmänvalvoja voi määrittää tilin käyttöoikeuden seuraavasti:

1. Avaa [Microsoft 365 -hallintakeskus,](https://portal.office.com/adminportal/home#/homepage) siirry  Aktiiviset käyttäjät -osioon ja valitse käyttäjä, joka näkee virheen. 

2. Siirry käyttäjäsivulla Käyttöoikeudet ja  sovellukset -osaan, valitse asianmukainen Sijainti-arvo ja määritä käyttöoikeus, joka sisältää Exchange Onlinen (laajenna käyttöoikeus, jotta näet sen tiedot).  Kun olet valmis, valitse **Tallenna muutokset.**

Joissakin tapauksissa, jos käyttöoikeus on jo määritetty käyttäjätilille, käyttöoikeuden poistaminen ja uudelleennimeäminen auttaa ratkaisemaan ongelman ja valmistella sen oikein järjestelmässä: 

- Tarkista, ovatko M365 Exchange Online -tilauksesi (ja muut, jos sinulla on) tilaukset ajan tasalla ja eivät ole hiljattain vanhentuneet.

Kun olet varmistanut, että tilauksesi ei ole päättynyt ja että käyttäjätilille on määritetty kelvollinen käyttöoikeus, käyttöoikeuden valmistelu voi kestää jopa 24 tuntia, joten sinun on ehkä odotettava ongelman ratkaisemista. Lisätietoja on kohdassa [Käyttöoikeuksien määrittäminen ja hallinta.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)