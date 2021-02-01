---
title: Tunnistetietoihin liittyvät ongelmat
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063628"
---
# <a name="issues-with-credentials"></a>Tunnistetietoihin liittyvät ongelmat

[Microsoftin tunnistetietoympäristössä ja OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) -asiakastietojen työnkulussa kuvataan, miten ohjelma voidaan ohjelmoida suoraan OAuth 2.0 -asiakastietojen grant flow -tunnuksen avulla.

**Miten hallitsen sovelluksen salasanaa tai varmenteen tunnistetietoja?**

Azure CLI:ssä voit [käyttää az ad -sovelluksen](https://docs.microsoft.com/cli/azure/ad/app/credential) tunnistetietoja sovelluksen salasanan tai varmenteen tunnistetietojen poistamiseen, luetteloon tai palauttamiseen.

**Miten käyttäjät palauttavat salasanansa?**

Käyttäjien on [rekisteröitävä omatoiminen salasanan vaihto,](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) ennen kuin he voivat vaihtaa salasanansa. Kun käyttäjä on rekisteröitynyt, hän voi palauttaa salasanansa noudattamalla tämän artikkelin ohjeita: Vaihda [työ- tai koulusalasanasi.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Miten käyttäjät vaihtavat salasanansa?**

Käyttäjät voivat vaihtaa salasanansa noudattamalla tässä artikkelissa annettuja ohjeita: [Salasanan vaihtaminen.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
He voivat myös [hallita sovelluksen salasanoja kaksivaiheista vahvistusta varten.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Käyttäjäni saa virheilmoituksen, kun salasanaa muutetaan tai palautetaan**

Tämä linkki antaa tietoja yleisistä ongelmista, joita voi ilmetä, kun käyttäjä yrittää vaihtaa salasanansa: yleisiä [ongelmia ja heidän ratkaisujaan](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Minulla on ongelmia käyttäjän salasanan palauttamisessa**

- Varmista, että sinulla on oikeus vaihtaa salasanoja. *Vain yleiset järjestelmänvalvojat, salasanat ja käyttäjien järjestelmänvalvojat voivat vaihtaa käyttäjien salasanat.* Yleiset järjestelmänvalvojat voivat myös palauttaa muiden järjestelmänvalvojan salasanat.

- Varmista, että ymmärrät käyttöoikeusvaatimukset:

  - Sinulla on oltava vähintään yksi käyttöoikeus määritettynä organisaatiossasi:
    - **Vain pilvipalvelun käyttäjät** – mikä tahansa Office 365 (O365) maksettu SKU tai Azure AD Basic
    - **Pilvi- ja/tai paikalliskäyttäjät** – Azure AD Premium P1 tai P2, Enterprise Mobility + Security (EMS) tai Secure Productive Enterprise (SPE)
    - Lisätietoja käyttöoikeusvaatimuksista on kohdassa [Azure AD:n omatoimista salasanan vaihtoa koskevat käyttöoikeusvaatimukset.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Jos haluat vaihtaa käyttäjän salasanan, etsi käyttäjä Azure AD:ssä. Napsauta sitten käyttäjän yleiskatsausterässä Palauta salasana -painiketta.

**Salasanan vaihtopainike näkyy harmaana**

Sinulla ei ole oikeutta **palauttaa** tämän käyttäjän salasanoja. *Vain yleiset järjestelmänvalvojat, salasanat ja käyttäjien järjestelmänvalvojat voivat vaihtaa käyttäjien salasanat.* Yleiset järjestelmänvalvojat voivat myös palauttaa muiden järjestelmänvalvojan salasanat.

**Salasanan vaihto-osaa ei ole**

Sinulla ei ole oikeutta vaihtaa salasanoja. *Vain yleiset järjestelmänvalvojat, salasanat ja käyttäjien järjestelmänvalvojat voivat vaihtaa käyttäjien salasanat.* Yleiset järjestelmänvalvojat voivat myös palauttaa muiden järjestelmänvalvojan salasanat.

**En näe paikallisen integroinnin teriä salasanan nollaamisen aikana**

- Paikallinen integrointisuljenta näkyy vain yhdistelmäympäristöissä, eli käytät salasanan palautusta paikallisen käyttäjän salasanojen käsittelemiseen.

- Et näe tätä terää, jos:

  - Et käytä salasanan palautusta
  - Salasanan takaisin kirjoittamisen asennuksessa ja yhteydessä on ongelma
  - Azure AD Connectin asennuksessa ja yhteydessä on ongelma
  - Lisätietoja salasanojen palautusongelmien vianmäärityksestä on ohjeaiheessa Salasanalla [kirjoitettavan takaisin kirjoittamisen vianmääritys](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**En tiedä, miten voin vaihtaa käyttäjän salasanan**

1. Kirjaudu Azure-portaaliin asianmukaisena järjestelmänvalvojana.
2. Siirry Käyttäjät ja **ryhmät -teriin** ja valitse **Kaikki käyttäjät.**
3. Valitse käyttäjä luettelosta.
4. Valitse valitulle käyttäjälle **Yleiskatsaus** ja valitse sitten komentopalkissa Palauta **salasana.**
5. Valitse Palauta **salasana -painike** ja noudata näyttöön tulevia ohjeita.
    - Vain Azure-portaalin kautta suoritetut **nollaukset tukevat** salasanan palautusta.

**Palautan paikallisen käyttäjän salasanan Office 365 -hallintaportaalista tai Office 365 -mobiilisovelluksesta, mutta käyttäjä ei vieläkään pysty kirjautumaan sisään**

Salasanasuojaa ei tueta tässä portaalissa. Palauta käyttäjän salasana uudelleen Azure-portaalissa.
