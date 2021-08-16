---
title: 126 Postilaatikon saamisvirhettä ei löydy OWA:sta?
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
ms.openlocfilehash: aca0371dad9ba43fa21b0df8e50f1b8ee536528af90d6bda401995c6e5796be4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54056487"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Saatko postilaatikon virhettä Outlookin verkkoversio?

Jos käytät Outlookin verkkoversio mutta saat virheilmoituksen  postilaatikosta, tiliä, jota käytit yhteyden muodostamisessa Outlookin verkkoversio:han, ei ole Exchange Online-käyttöoikeutta eikä näin ollen postilaatikkoa ole liitetty tiliin. Järjestelmänvalvoja voi määrittää tilin käyttöoikeuden seuraavasti:

1. Avaa [Microsoft 365 -hallintakeskus,](https://portal.office.com/adminportal/home#/homepage) siirry **Aktiiviset käyttäjät** -kohtaan Käyttäjät-osassa ja valitse käyttäjä, joka näkee virheen. 

2. Siirry käyttäjäsivulla Käyttöoikeudet ja  sovellukset -osaan, valitse asianmukainen Sijainti-arvo ja määritä käyttöoikeus, joka sisältää Exchange Online (laajenna käyttöoikeus, jotta näet sen tiedot).  Kun olet valmis, valitse **Tallenna muutokset**.

Joissakin tapauksissa, jos käyttöoikeus on jo määritetty käyttäjätilille, käyttöoikeuden poistaminen ja uudelleennimeäminen auttaa ratkaisemaan ongelman ja valmistella sen oikein järjestelmässä: 

- Tarkista, ovatko M365 -tilauksesi Exchange Online (ja muut, jos sinulla on) tilaukset ovat ajan tasalla ja eivät ole hiljattain vanhentuneet.

Kun olet varmistanut, että tilauksesi ei ole päättynyt ja että käyttäjätilille on määritetty voimassa oleva käyttöoikeus, käyttöoikeuden valmistelu voi kestää jopa 24 tuntia, joten sinun on ehkä odotettava ongelman ratkaisemista. Lisätietoja on kohdassa [Käyttöoikeuksien määrittäminen ja hallinta.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)