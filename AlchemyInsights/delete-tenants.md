---
title: Vuokra ajan poistaminen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564484"
---
# <a name="delete-tenant"></a>Vuokra ajan poistaminen

Jos haluat poistaa Azure-mainoksen, varmista seuraavat:
- Olet hakemiston yleinen hallinnoija.
- Et ole kirjautunut tilillä, joka sisältää oletus hakemiston, kuten contoso.onmicrosoft.com, kirjautuneen tilin, kuten admin@contoso.onmicrosoft.com.
- Poista kaikki kansiossa olevat aktiiviset sovellukset ennen niiden poistamista. Jos haluat poistaa aktiivisia sovelluksia, siirry sovellusten rekisteröinteihin ja poista olemassa olevat sovellukset.
- Minkään Microsoft Online-palvelun, kuten Microsoft Azuren, Office 365 tai Azuren AD Premiumin, käytössä ei ole aktiivisia paketteja. Siirrä tilauksesi tai nopeuta aktiivisten pakettien peruutusta Azure-tuen ja laskutuksen kautta. Lue lisää siitä, miten voit peruuttaa Office 365-ja Azure-tila uksia. Lisä tietoja olemassa olevan tila uksen liittämisestä vuokraajaan on Ohje aiheessa Azure- [tila uksen liittäminen tai lisääminen Azure AD-vuokraajaan](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Aktiivista käyttö oikeutta ei ole. Lisä tietoja käyttö oikeuksien poistamisesta on Ohje aiheessa [tila uksen poistaminen käyttö oikeuden poistamiseksi](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Hakemistossa ei ole muita aktiivisia käyttäjiä paitsi itseäsi yleisenä järjestelmänvalvojana, kun yrität poistaa Azure AD:n. Poista kaikki muut aktiiviset käyttäjät, ja mukautetun toimi alue nimen riippuvuudet on myös poistettava, kuten admin@contoso.com-sovelluksessa luodut käyttäjät.

Lisä tietoja:
- Poista Azure Active Directory tai tilaus, Katso lisä tietoja artikkelista [Azure Active Directoryn poistaminen](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Sovellusten poistaminen hakemistosta on kohdassa [sovellusten poistaminen](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
