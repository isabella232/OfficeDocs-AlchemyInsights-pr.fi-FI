---
title: Mitä tehdä, jos Azure-ominaisuudet eivät toimi oikein Microsoft Edgessä
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583463"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Mitä tehdä, jos Azure-ominaisuudet eivät toimi oikein Microsoft Edgessä

Microsoft Edgessä on [tunnettuja ongelmia](https://go.microsoft.com/fwlink/?linkid=2140608) , jotka liittyvät turva vyöhykkeisiin ja saattavat vaikuttaa siihen, miten Azure-käyttäjät kirjautuvat Windows Admin Centeriin. Jos sinulla on ongelmia Azure-ominaisuuksien käyttämisessä Microsoft Edgessä, kokeile seuraavia vaiheita:

1. Etsi **Käynnistä** -valikosta **Internet-asetukset** ja valitse se.
2. Valitse **Internet-ominaisuudet** -valinta ikkunassa **turvallisuus** -väli lehti.
3. Valitse **Luotetut sivustot** -vyöhyke ja valitse sitten **sivustot** -painike.
4. Lisää **Luotetut sivustot** -valinta ikkunaan yhdyskäytävän URL-osoite sekä [https://login.microsoftonline.com](https://login.microsoftonline.com) ja ja [https://login.live.com](https://login.live.com) Valitse sitten **Sulje**.
5. Valitse **Internet-ominaisuudet** -valinta ikkunassa **tieto suoja** -väli lehti.
6. Valitse **ponnahdus ikkunoiden esto-** osassa **Asetukset**. Lisää avautuvaan valinta ikkunaan yhdyskäytävän URL-osoite sekä [https://login.microsoftonline.com](https://login.microsoftonline.com) ja ja [https://login.live.com](https://login.live.com) Valitse sitten **Sulje**.
