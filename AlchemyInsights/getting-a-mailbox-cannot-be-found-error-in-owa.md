---
title: 126 Postilaatikon hakeminen ei ole virhe OWA:ssa?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 4/9/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: e061ad6b74b27e3f0d597586cb2c8e31b8fa5d23
ms.sourcegitcommit: 83c644c35c2700dc515f091c8f41f9c283b89967
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2020
ms.locfileid: "43105236"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Saatko postilaatikon, joka ei ole löytynyt -virheestä Outlookin verkkoversiossa?

Jos käytät Outlookin verkkoyhteyttä ja **postilaatikkoa ei löytynyt virheeksi,** tilillä, jolla muodostat yhteyden Outlookin verkkoversioon, ei ole Exchange Online -käyttöoikeutta, joten tiliin ei ole liitetty postilaatikkoa. Järjestelmänvalvoja voi määrittää tiliisi käyttöoikeuden seuraavasti:

1. Avaa [Microsoft 365 -hallintakeskus](https://portal.office.com/adminportal/home#/homepage) ja siirry **Käyttäjät-osan** **Aktiiviset käyttäjät** -kohtaan ja valitse käyttäjä, joka näkee virheen.

2. Siirry avautuvan käyttäjäsivun Käyttöoikeudet **ja sovellukset -osaan,** valitse asianmukainen **Sijainti-arvo** ja määritä Käyttöoikeus, joka sisältää Exchange Onlinen (laajenna käyttöoikeus nähdäksesi sen tiedot). Kun olet valmis, valitse **Tallenna muutokset**.
