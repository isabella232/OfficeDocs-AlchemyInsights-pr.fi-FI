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
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986816"
---
# <a name="issues-with-credentials"></a>Tunnistetietoihin liittyvät ongelmat

[Microsoftin käyttäjätietoympäristö ja OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) -asiakastietojen työnkulussa kuvataan, miten ohjelma voidaan ohjelmoida suoraan OAuth 2.0 -asiakastietojen grant flow -työnkulun avulla.

**Miten hallitsen sovelluksen salasanaa tai varmenteen tunnistetietoja?**

Azure CLI:ssä voit käyttää [az ad -sovelluksen](https://docs.microsoft.com/cli/azure/ad/app/credential) tunnistetietoja sovelluksen salasanan tai varmenteen tunnistetietojen poistamiseen, luetteloon tai palauttamiseen.

**Miten käyttäjät palauttavat salasanansa?**

Käyttäjien on [rekisteröitävä omatoiminen salasanan vaihto,](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) ennen kuin he voivat vaihtaa salasanansa. Kun käyttäjä on rekisteröity, hän voi palauttaa salasanansa noudattamalla tässä artikkelissa annettuja ohjeita: [Palauta työ- tai koulusalasana.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Miten käyttäjät vaihtavat salasanansa?**

Käyttäjät voivat vaihtaa salasanansa noudattamalla tässä artikkelissa annettuja ohjeita: [Salasanan vaihtaminen.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
He voivat myös [hallita sovelluksen salasanoja kaksivaiheista tarkistamista varten.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Käyttäjäni saa virheilmoituksen salasanan vaihtamisen tai vaihtamisen jälkeen**

Tämä linkki antaa tietoja yleisistä ongelmista, joita voi ilmetä, kun käyttäjä yrittää vaihtaa salasanansa: yleisiä ongelmia [ja heidän ratkaisujaan](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Minulla on ongelmia käyttäjän salasanan palauttamisessa**

- Varmista, että sinulla on oikeus vaihtaa salasanoja. *Vain yleiset järjestelmänvalvojat, salasanat ja käyttäjien järjestelmänvalvojat voivat vaihtaa käyttäjien salasanat.* Yleiset järjestelmänvalvojat voivat myös palauttaa muiden järjestelmänvalvojien salasanat.

- Varmista, että ymmärrät käyttöoikeusvaatimukset:

  - Organisaatiossasi on oltava määritettynä vähintään yksi käyttöoikeus:
    - **Vain pilvikäyttäjät** – mikä tahansa Office 365 (O365) maksettu SKU tai Azure AD Basic
    - **Pilvi- ja/tai paikalliskäyttäjät** – Azure AD Premium P1 tai P2, Enterprise Mobility + Security (EMS) tai Secure Productive Enterprise (SPE)
    - Lisätietoja käyttöoikeusvaatimuksista on kohdassa [Azure AD:n omatoimista salasanan vaihtoa koskevat käyttöoikeusvaatimukset.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Jos haluat vaihtaa käyttäjän salasanan, etsi käyttäjä Azure AD:ssä. Napsauta sitten käyttäjän yleiskatsauksen lapaa ja napsauta "Vaihda salasana" -painiketta.

**Salasanan vaihtopainike näkyy harmaana**

Sinulla ei ole oikeutta **vaihtaa** tämän käyttäjän salasanoja. *Vain yleiset järjestelmänvalvojat, salasanat ja käyttäjien järjestelmänvalvojat voivat vaihtaa käyttäjien salasanat.* Yleiset järjestelmänvalvojat voivat myös palauttaa muiden järjestelmänvalvojien salasanat.

**En näe salasanan vaihto-osaa**

Sinulla ei ole oikeutta vaihtaa salasanoja. *Vain yleiset järjestelmänvalvojat, salasanat ja käyttäjien järjestelmänvalvojat voivat vaihtaa käyttäjien salasanat.* Yleiset järjestelmänvalvojat voivat myös palauttaa muiden järjestelmänvalvojien salasanat.

**I don't see the on-premises integration blade in password reset**

- Paikallisen integroinnin laita näkyy vain yhdistelmäympäristöissä, eli käytät salasanan palautusta paikallisen käyttäjän salasanojen käsittelemiseen.

- Et näe tätä lapaa, jos:

  - Et käytä salasanan kirjoitusta takaisin
  - Salasanalla kirjoittamisen asennuksessa ja yhteydessä on ongelma
  - Azure AD Näyttöyhteys:n asennuksessa tai yhteydessä on Näyttöyhteys
  - Lisää vianmääritysohjeita salasanan takaisin kirjoittamisen ongelmiin on ohjeaiheessa [Salasanaan kirjoittamisen vianmääritys](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**En tiedä, miten käyttäjän salasanan voi vaihtaa**

1. Kirjaudu Azure-portaaliin asianmukaisena järjestelmänvalvojana.
2. Siirry Käyttäjät **ja ryhmät -teriin** ja valitse **Kaikki käyttäjät**.
3. Valitse käyttäjä luettelosta.
4. Valitse valitun käyttäjän yleiskatsaus **ja** valitse sitten komentopalkissa **Vaihda salasana**.
5. Valitse **Palauta salasana** -painike ja noudata näyttöön tulevia ohjeita.
    - Vain Azure-portaalin kautta suoritetut **nollaukset tukevat** salasanan palautusta.

**Palautan paikallisen käyttäjän salasanan Office 365:n hallintasovellus-portaalista tai Office 365 mutta käyttäjä ei vieläkään pysty kirjautumaan sisään**

Tässä portaalissa ei tueta salasanan kirjoitusta. Palauta käyttäjän salasana uudelleen Azure-portaalissa.
