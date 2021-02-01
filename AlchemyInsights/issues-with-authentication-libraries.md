---
title: Todentamiskirjastoihin liittyvät ongelmat
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063606"
---
# <a name="issues-with-authentication-libraries"></a>Todentamiskirjastoihin liittyvät ongelmat

1. [Microsoftin käyttäjätietoympäristön todennuskirjastoissa](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) on luettelo Microsoftin tukemista ja yhteensopivista asiakas- ja middleware-kirjastoista.
2. Microsoftin todentamiskirjasto (MSAL) tukee useita [todennusvirtoja](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) käytettäväksi eri sovellusskenaarioissa.
3. Jos haluat todentaa ja hankkia tunnuksia, alusta uusi julkinen tai luottamuksellinen asiakassovellus koodissasi. Voit määrittää useita määritysasetuksia, kun alustat asiakassovelluksen Microsoftin todennuskirjastossa (MSAL). Lisätietoja on kohdassa Sovelluksen [määritysasetukset.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Azure Active Directory -todennuskirjaston (ADAL) ja Azure AD Graph API:n (AAD Graph) tuen päättyminen**

**30. kesäkuuta 2020** alkaen uusia ominaisuuksia ei enää lisätä ADAL:een ja Azure AD Graphiin. Tarjoamme jatkossakin teknistä tukea ja suojauspäivityksiä, mutta emme enää tarjoa ominaisuuspäivityksiä.

**30. kesäkuuta 2022** alkaen microsoft lopettaa ADAL: n ja Azure AD Graphin tuen, eikä se enää tarjoa teknistä tukea tai suojauspäivityksiä.

Sovellukset, jotka käyttävät ADAL:tä nykyisissä käyttöjärjestelmäversioissa, toimivat edelleen tämän ajan kuluttua, mutta eivät saa *teknistä tukea tai suojauspäivityksiä.*

Azure AD Graphia tämän jälkeen käyttävät sovellukset eivät ehkä enää saa vastauksia Azure AD Graph -päätepisteltä.

**ADAL-siirto**

Suosittelemme päivittämistä [Microsoft todentamiskirjastoon (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), jossa on uusimmat ominaisuudet ja suojauspäivitykset.

Jos käytät Microsoft-sovelluksia, tiedät, että Microsoft on parhaillaan muuttamassa sovelluksiaan MSAL-sovelluksiin tuen päättymiseen mennessä, jotta ne hyötyvät MSAL:n käynnissä olevista suojaus- ja ominaisuusparannuksista.

Lisätietoja on seuraavissa artikkeleissa:

1. [Lue ADAL:ää koskevat usein kysytyt kysymykset](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Lisätietoja sovellusten siirtämisestä käyttöympäristökohtaisesti](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Jos tarvitset apua sen ymmärtämiseen, mitkä sovellukset käyttävät ADAL:tä, suosittelemme tarkistamaan kaikki sovellusten lähdekoodit ja tarvittaessa ottaa yhteyttä internet-palveluntarjoajiin tai sovellustarjoajiin. Microsoftin tukipalvelu voi myös tarjota sinulle luettelon kaikista vuokraajan ei-Microsoft ADAL -sovelluksista.

**AAD Graph -siirto**

Jos sovellus käyttää Azure AD Graphia, noudata ohjeita azure AD Graph -sovellusten [siirtämiseksi Microsoft Graphiin.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Siirron tarkistusluettelomme tarjoaa aloituspisteen.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Azure-sovelluksen rekisteröintiportaali näyttää, mitkä sovellukset käyttävät AAD Graphia. Suosittelemme, että tarkistat kaikki sovellusten lähdekoodit. Ota tarvittaessa yhteyttä internet-palveluntarjoajaan tai sovelluksen toimittajaan. Microsoft-tuki voi myös tarjota sinulle luettelon vuokraajan kaikista AAD Graph -käytöstä.
3. Jotta sovellus voi käyttää Microsoft Graphin tietoja, käyttäjän tai järjestelmänvalvojan on myönnettävä se oikeat käyttöoikeudet suostumusprosessin kautta. [Microsoft Graph -käyttöoikeusviittauksessa](https://docs.microsoft.com/graph/permissions-reference) luetellaan kuhunkin Microsoft Graph -ohjelmointirajapintojen pääjoukkoon liittyvät käyttöoikeudet. Artikkelissa on myös ohjeita käyttöoikeuksien käyttöön.
