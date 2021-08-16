---
title: Ongelmia salasanan vaihtamisessa
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039963"
---
# <a name="problems-resetting-password"></a>Ongelmia salasanan palauttamisessa

Seuraavassa on joitakin ongelmia, joita saatat kohdata salasanan vaihtamisen jälkeen, ja mahdollisia ratkaisuja:

**Minulla on ongelmia salasanan palauttamisessa, jota ei ole käsitelty muissa luokissa**

- Varmista, että sinulla on oikeus vaihtaa salasanoja. Vain yleiset järjestelmänvalvojat, salasanat ja käyttäjien järjestelmänvalvojat voivat vaihtaa käyttäjien salasanat. Yleiset järjestelmänvalvojat voivat myös palauttaa muiden järjestelmänvalvojien salasanat.
- Varmista, että ymmärrät käyttöoikeusvaatimukset:
    - Sinulla on oltava vähintään yksi käyttöoikeus määritettynä organisaatiossasi
        - Vain pilvikäyttäjät – mikä tahansa Office 365 (O365) maksettu SKU tai Azure AD Basic
        - Pilvi- ja/tai paikalliskäyttäjät – Azure AD Premium P1 tai P2, Enterprise Mobility + Security (EMS) tai Secure Productive Enterprise (SPE)
        - Lisätietoja käyttöoikeusvaatimuksista on artikkelissa [Azure AD:n omatoimista salasanan vaihtoa koskevat käyttöoikeusvaatimukset.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Minulla on ongelmia asettamani salasanan vaihtokäytännön testaamiseen**

- Äskettäin käytetyt käytännöt voivat replikoida kaikissa tietokeskuksissa ja päätepisteissä useita minuutteja. Fyysinen etäisyys tietokeskuksesta vaikuttaa myös siihen, miten nopeasti muutokset otetaan käyttöön.
- Testaa loppukäyttäjän, ei järjestelmänvalvojan, kanssa ja pilotaa pienen käyttäjäjoukon kanssa. Azure-portaalissa määritetyt käytännöt koskevat VAIN loppukäyttäjiä, eivät järjestelmänvalvojille. Microsoft ottaa käyttöön vahvan kaksiportaisen salasanan vaihtokäytännön kaikissa Azure-järjestelmänvalvojien roolissa (esimerkki: yleinen järjestelmänvalvoja, tukipalvelun järjestelmänvalvoja, salasanan järjestelmänvalvoja jne.)
    - Lisätietoja [järjestelmänvalvojien käytännöistä.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Haluan ottaa käyttöön salasanan palauttamisen, mutta en halua, että käyttäjät rekisteröivät muita suojaustietoja**

Esitä käyttäjien tiedot, jotta heidän ei tarvitse tehdä sitä. - Järjestelmänvalvojana voit määrittää käyttäjille puhelin- ja sähköpostiominaisuudet ennen kuin otat salasanan palauttamisen käyttöön organisaatiossasi. Voit tehdä tämän ohjelmointirajapinnan, PowerShellin tai Azure AD:n Näyttöyhteys. Lisätietoja on täällä:
- [Salasanan palauttamisen käyttöönotto ilman, että käyttäjien on rekisteröidyttävä](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Mitä tietoja salasanan nollaaminen käyttää](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Salasanan vaihtopainike näkyy harmaana**

Sinulla ei ole oikeutta vaihtaa tämän käyttäjän salasanoja. Vain yleiset järjestelmänvalvojat, salasanat ja käyttäjien järjestelmänvalvojat voivat vaihtaa käyttäjien salasanat. Yleiset järjestelmänvalvojat voivat myös palauttaa muiden järjestelmänvalvojien salasanat.

**En näe salasanan vaihto-osaa**

Sinulla ei ole oikeutta vaihtaa salasanoja. Vain yleiset järjestelmänvalvojat, salasanat ja käyttäjien järjestelmänvalvojat voivat vaihtaa käyttäjien salasanat. Yleiset järjestelmänvalvojat voivat myös palauttaa muiden järjestelmänvalvojien salasanat.

**I don't see the on-premises integration blade in password reset**

- Paikallisen integroinnin laita näkyy vain yhdistelmäympäristöissä, eli käytät salasanan palautusta paikallisen käyttäjän salasanojen käsittelemiseen.
- Et näe tätä lapaa, jos:
    - Et käytä salasanan kirjoitusta takaisin
    - Salasanalla kirjoittamisen asennuksessa ja yhteydessä on ongelma
    - Azure AD Näyttöyhteys:n asennuksessa tai yhteydessä on Näyttöyhteys
    - Lisätietoja salasanan takaisin kirjoittaminen -ongelmien vianmäärityksestä on kohdassa Salasanan takaisin [kirjoittamisen vianmääritys](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**En tiedä, miten käyttäjän salasanan voi vaihtaa**

1. Kirjaudu Azure-portaaliin asianmukaisena järjestelmänvalvojana.
1. Siirry Käyttäjät ja ryhmät -teriin ja valitse **Kaikki käyttäjät**.
1. Valitse käyttäjä luettelosta.
1. Valitse valitun käyttäjän yleiskatsaus **ja** valitse sitten komentopalkissa **Vaihda salasana**.
1. Noudata näyttöön tulevia ohjeita.
    - Vain Azure-portaalin kautta suoritetut nollaukset tukevat salasanan palautusta.

**Palautan paikallisen käyttäjän salasanan Office 365:n hallintasovellus-portaalista tai Office 365 mutta käyttäjä ei vieläkään pysty kirjautumaan sisään**

Tässä portaalissa ei tueta salasanan kirjoitusta. Käyttäjän salasanan palauttaminen uudelleen Azure-portaalissa – portal.azure.com

