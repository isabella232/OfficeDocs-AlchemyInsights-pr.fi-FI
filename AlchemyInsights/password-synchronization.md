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
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481446"
---
# <a name="password-synchronization"></a>Salasanan synkronoiminen

**Salasanojen hash-synkronointi ei toimi lainkaan**

Joitakin yleisiä ongelmia, joita asiakkaat kohtaavat, kun salasanojen hash-synkronointi ei toimi, ovat:

- Azure AD Connectin paikallisen Active Directory -yhteyden muodostamiseen käyttämälle  Active Directory  -tilille ei myönnetä replikoida hakemistomuutoksia ja replikoida hakemistomuutoksia, joten kaikki salasanasynkronoinnin edellyttämät käyttöoikeudet on korjattava myöntämällä nämä käyttöoikeudet Active Directory -tilille.
- Salasanojen hash-synkronointi poistetaan käytöstä, kun järjestelmänvalvoja  on vaihtanut User Sign-In -menetelmän salasanasynkronoinnista toiseen vaihtoehtoon, kuten liittounnin **AD FS:ään** ohjatussa Azure AD Connect -toiminnossa . Voit korjata ongelman ottamalla salasanojen **hash-synkronointitoiminnon** uudelleen käyttöön ohjatussa Azure AD Connect -toiminnossa.
- Paikallisen Active Directoryn yhteysongelma. Esimerkiksi jotkin toimialueen ohjauskoneet eivät ole Azure AD [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) Connectin käytettävissä, tai palomuuri estää vaaditut portit. Tämä on korjattava varmistamalla, että Azure AD Connect -palvelimen ja paikallisen Active Directoryn välinen yhteys toimii oikein.
- Azure AD Connect -palvelin on parhaillaan valmistelutilassa, jolloin palvelin ei voi käyttää salasanojen sulkuja. Voit ratkaista ongelman noudattamalla osiossa [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)-synkronoinnin salasanojen synkronoinnin vianmääritys - Salasanoja ei synkronoida.

**Salasanojen hash-synkronointi ei toimi joillakin käyttäjillä**

1. Jos olet huomannut, että salasanan hash ei synkronoidu  käyttäjälle, voit tutkia ja ratkaista ongelman Azure AD Connectin vianmääritystehtävän avulla. Suorita seuraavat tehtävät:

    a. [Suorita vianmääritystehtävä ohjatussa toiminnossa](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Salasanan hash-synkronointiongelman tutkiminen tietyssä käytössä cmdlet-vianmäärityksen cmdlet-komentoa käyttämällä](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Paikallisen Active Directory -käyttäjäobjektin on oltava käytössä käyttäjän on vaihdettava salasana **seuraavalla kirjautumisvaihtoehdolla.** Kun tämä asetus on käytössä, käyttäjälle määritetään tilapäinen salasana, ja sinua pyydetään vaihtamaan salasana seuraavassa kirjautumisessa. Azure AD Connect ei synkronoi tilapäisiä salasanoja Azure AD:n kanssa.

Voit ratkaista edellä mainitun ongelman jommankumman seuraavista tehtävistä:

- Pyydä käyttäjää kirjautumaan paikalliseen sovellukseen (esimerkiksi Windows-työpöydälle) ja vaihtamaan salasana. Uusi salasana synkronoidaan Azure AD:n kanssa.
- Järjestelmänvalvoja voi päivittää käyttäjän salasanan ilman, että käyttäjän on vaihdettava salasana seuraavalla kirjautumista **varten,** ja jakamaan uusi salasana käyttäjän kanssa.

3. Paikallisen Active Directory -käyttäjän objektia ei **ole määritetty oikein objektisynkronointia** tai salasanasynkronointia varten. Voit tehdä vianmäärityksen noudattamalla artikkelissa Salasanojen hash-synkronoinnin vianmääritys [Azure AD Connect -synkronoinnin kanssa annettuja ohjeita.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







