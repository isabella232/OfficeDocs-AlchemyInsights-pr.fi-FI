---
title: Salasanan synkronoiminen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960832"
---
# <a name="password-synchronization"></a>Salasanan synkronoiminen

**Salasanojen hash-synkronointi ei toimi lainkaan**

Asiakkaat kohtaavat joitakin yleisiä ongelmia, kun salasanojen hash-synkronointi ei toimi:

- Azure AD Näyttöyhteys:n paikalliseen Active Directoryyn viestimiseen käyttämälle Active  Directory -tilille  ei myönnetä Replikoi hakemistomuutoksia ja Replikoi hakemistomuutokset Kaikki salasanasynkronoinnin edellyttämät käyttöoikeudet . Tämä on korjattava myöntämällä nämä oikeudet Active Directory -tilille.
- Salasanojen hash-synkronointi poistetaan käytöstä sen jälkeen, kun  järjestelmänvalvoja on vaihtanut User Sign-In -menetelmän salasanasynkronoinnista toiseen vaihtoehtoon, kuten liittounnin **AD FS:ään** ohjatussa Azure AD Näyttöyhteys -toiminnossa – Voit korjata ongelman ottamalla salasanojen **hash-synkronointitoiminnon** uudelleen käyttöön ohjatussa Azure AD Näyttöyhteys -toiminnossa.
- Paikallisen Active Directoryn yhteysongelma. Esimerkiksi jotkin toimialueen ohjauskoneet eivät ole Azure AD Näyttöyhteys:n [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) käytettävissä, tai palomuuri estää vaaditut portit. Tämä on korjattava varmistamalla, että Azure AD Näyttöyhteys -palvelimen ja paikallisen Active Directoryn välinen yhteys toimii oikein.
- Azure AD Näyttöyhteys -palvelin on parhaillaan valmistelutilassa, minkä vuoksi palvelin ei voi käyttää salasanojen sulkuja. Voit tehdä ongelman vianmäärityksen noudattamalla kohdassa Salasanasynkronoinnin vianmääritys [Azure AD Näyttöyhteys](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)-synkronoinnin kanssa - Salasanoja ei synkronoida.

**Salasanojen hash-synkronointi ei toimi joillakin käyttäjillä**

1. Jos huomasit, että salasanojen hash ei synkronoidu  käyttäjän kanssa, voit tutkia ja ratkaista Näyttöyhteys Azure AD:n vianmääritystehtävän avulla. Suorita seuraavat tehtävät:

    a. [Suorita vianmääritystehtävä ohjatussa toiminnossa](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Salasanan hash-synkronointiongelman tutkiminen vianmääritys-cmdlet-komentoa käyttämällä](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Paikallisen Active Directory -käyttäjän objekti on otettu käyttöön Käyttäjän on vaihdettava **salasana seuraavalla kirjautumisvaihtoehdolla.** Kun tämä asetus on käytössä, käyttäjälle määritetään tilapäinen salasana, ja ohjelma pyytää vaihtamaan salasanan seuraavalla kirjautumista varten. Azure AD Näyttöyhteys synkronoi tilapäisiä salasanoja Azure AD:lle.

Voit ratkaista edellä mainitun ongelman jommankumman seuraavista tehtävistä:

- Pyydä käyttäjää kirjautumaan paikalliseen sovellukseen (esimerkiksi Windows) ja vaihtamaan salasana. Uusi salasana synkronoidaan Azure AD:n kanssa.
- Anna järjestelmänvalvojan päivittää käyttäjän salasana ottamalla käyttöön asetusta Käyttäjän on vaihdettava salasana seuraavalla kirjautumista varten ja jakamatta uutta salasanaa käyttäjän kanssa.

3. Paikallisen Active Directory -käyttäjän objektia ei ole **määritetty oikein objektien** synkronointia tai salasanojen synkronointia varten. Voit tehdä vianmäärityksen noudattamalla artikkelissa Salasanojen hash-synkronoinnin vianmääritys Azure AD:n kanssa Näyttöyhteys [ohjeita.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







