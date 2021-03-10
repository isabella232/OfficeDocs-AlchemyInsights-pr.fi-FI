---
title: Ongelma salasanan vaihtamisessa
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
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694374"
---
# <a name="problems-resetting-password"></a>Ongelmia salasanan vaihtamisessa

Seuraavassa on joitakin ongelmia, joita saatat kohdata salasanan vaihtamisen ja mahdollisia ratkaisuja käytettäessä:

**Minulla on ongelmia salasanan palauttamisessa, jota ei ole käsitelty muissa luokissa**

- Varmista, että sinulla on oikeus vaihtaa salasanoja. Vain yleiset järjestelmänvalvojat, salasanat ja käyttäjien järjestelmänvalvojat voivat vaihtaa käyttäjien salasanat. Yleiset järjestelmänvalvojat voivat myös palauttaa muiden järjestelmänvalvojan salasanat.
- Varmista, että ymmärrät käyttöoikeusvaatimukset:
    - Sinulla on oltava vähintään yksi käyttöoikeus määritettynä organisaatiossasi
        - Vain pilvipalvelun käyttäjät – mikä tahansa Office 365 (O365) maksettu SKU tai Azure AD Basic
        - Pilvi- ja/tai paikalliskäyttäjät – Azure AD Premium P1 tai P2, Enterprise Mobility + Security (EMS) tai Secure Productive Enterprise (SPE)
        - Lisätietoja käyttöoikeusvaatimuksista on artikkelissa Azure AD:n omatoimista salasanan vaihtoa [koskevat käyttöoikeusvaatimukset.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**I'm having problems testing the password reset policy I set**

- Viimeksi käytetyt käytännöt voivat replikoida kaikissa tietokeskuksissa ja päätepisteissä useita minuutteja. Fyysinen etäisyys tietokeskuksesta vaikuttaa myös siihen, miten nopeasti muutoksia otetaan käyttöön.
- Testaa loppukäyttäjän, ei järjestelmänvalvojan, kanssa ja pilotaa pienen käyttäjäjoukon kanssa. Azure-portaalissa määritetyt käytännöt koskevat vain loppukäyttäjiä, eivät järjestelmänvalvojille. Microsoft käyttää vahvaa kahden portin oletussalasanan palautuskäytäntöä kaikissa Azure-järjestelmänvalvojan roolissa (esimerkki: yleinen järjestelmänvalvoja, tukipalvelun järjestelmänvalvoja, salasanan järjestelmänvalvoja jne.)
    - Lisätietoja [järjestelmänvalvojien käytännöistä.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Haluan ottaa salasanan palauttamisen käyttöön, mutta en halua, että käyttäjät rekisteröivät muita suojaustietoja**

Lisää käyttäjien tiedot valmiiksi, jotta heidän ei tarvitse! - Järjestelmänvalvojana voit määrittää käyttäjien puhelin- ja sähköpostiominaisuudet ennen salasanan palauttamisen käyttöönottamista organisaatiossasi. Voit tehdä tämän ohjelmointirajapinnan, PowerShellin tai Azure AD Connectin avulla. Lisätietoja on seuraavassa:
- [Salasanan palauttamisen käyttöönotto ilman, että käyttäjien on rekisteröidyttävä](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Mitä tietoja salasanan nollaaminen käyttää](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Salasanan vaihtopainike näkyy harmaana**

Sinulla ei ole oikeutta palauttaa tämän käyttäjän salasanoja. Vain yleiset järjestelmänvalvojat, salasanat ja käyttäjien järjestelmänvalvojat voivat vaihtaa käyttäjien salasanat. Yleiset järjestelmänvalvojat voivat myös palauttaa muiden järjestelmänvalvojan salasanat.

**I don't see the password reset blade**

Sinulla ei ole oikeutta vaihtaa salasanoja. Vain yleiset järjestelmänvalvojat, salasanat ja käyttäjien järjestelmänvalvojat voivat vaihtaa käyttäjien salasanat. Yleiset järjestelmänvalvojat voivat myös palauttaa muiden järjestelmänvalvojan salasanat.

**I don't see the on-premises integration blade in password reset**

- Paikallinen integrointisuljenta näkyy vain yhdistelmäympäristöissä, eli käytät salasanan palautusta paikallisen käyttäjän salasanojen käsittelemiseen.
- Et näe tätä terää, jos:
    - Et käytä salasanan palautusta
    - Salasanan takaisin kirjoittamisen asennuksessa ja yhteydessä on ongelma
    - Azure AD Connectin asennuksessa ja yhteydessä on ongelma
    - Lisätietoja salasanan palautusongelmien vianmäärityksestä on kohdassa Salasanan takaisin [kirjoittamisen vianmääritys](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**En tiedä, miten voin vaihtaa käyttäjän salasanan**

1. Kirjaudu Azure-portaaliin asianmukaisena järjestelmänvalvojana.
1. Siirry Käyttäjät ja ryhmät -teriin ja valitse **Kaikki käyttäjät.**
1. Valitse käyttäjä luettelosta.
1. Valitse valitulle käyttäjälle **Yleiskatsaus** ja valitse sitten komentopalkissa Palauta **salasana.**
1. Noudata näyttöön tulevia ohjeita.
    - Vain Azure-portaalin kautta suoritetut nollaukset tukevat salasanan palautusta.

**Palautan paikallisen käyttäjän salasanan Office 365 -hallintaportaalista tai Office 365 -mobiilisovelluksesta, mutta käyttäjä ei vieläkään pysty kirjautumaan sisään**

Salasanasuojaa ei tueta tässä portaalissa. Käyttäjän salasanan palauttaminen uudelleen Azure-portaalissa – portal.azure.com

