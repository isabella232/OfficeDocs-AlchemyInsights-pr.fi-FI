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
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028001"
---
# <a name="issues-with-authentication-libraries"></a>Todentamiskirjastoihin liittyvät ongelmat

1. [Microsoftin käyttäjätietoympäristö-kirjastoissa on](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) luettelo Microsoftin tukemista ja yhteensopivista asiakas- ja middleware-kirjastoista.
2. Microsoftin todentamiskirjasto (MSAL) tukee useita [todennusvirtoja](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) eri sovellusskenaarioissa käytettäväksi.
3. Todentaaksesi ja hankkiaksesi tunnuksia, sinun on alustanut uuden julkisen tai luottamuksellisen asiakassovelluksen koodissasi. Voit määrittää useita määritysasetuksia, kun alustat asiakassovelluksen Microsoftin todennuskirjastossa (MSAL). Lisätietoja on kohdassa Sovelluksen [määritysasetukset.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Azure Active Directory -todennuskirjaston (ADAL) ja Azure AD Graph -ohjelmointirajapinnan (AAD-Graph) tuen päättyminen**

**30. kesäkuuta 2020** alkaen uusia ominaisuuksia ei enää lisätä ADAL- ja Azure AD Graph. Tarjoamme jatkossakin teknistä tukea ja suojauspäivityksiä, mutta emme enää tarjoa ominaisuuspäivityksiä.

**30. kesäkuuta 2022** alkaen Microsoft lopettaa ADAL- ja Azure AD Graph ei enää tarjoa teknistä tukea tai suojauspäivityksiä.

Sovellukset, jotka käyttävät ADAL:tä olemassa olevissa käyttöjärjestelmäversioissa, toimivat edelleen tämän ajan kuluttua, mutta eivät saa *mitään teknistä tukea tai suojauspäivityksiä.*

Sovellukset, jotka käyttävät Azure AD Graph tämän ajan jälkeen, eivät ehkä enää saa vastauksia Azure AD Graph päätepisteltä.

**ADAL-siirto**

Suosittelemme päivittämistä [Microsoft todentamiskirjastoon (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), jossa on uusimmat ominaisuudet ja suojauspäivitykset.

Jos käytät Microsoft-sovelluksia, tiedät, että Microsoft on parhaillaan muuttamassa sovelluksiaan MSAL-sovelluksiin tuen päättymiseen mennessä, joten ne hyötyvät MSAL:n jatkuvia suojaus- ja ominaisuusparannuksia.

Lisätietoja on seuraavissa artikkeleissa:

1. [Lue ADAL:ää koskevat usein kysytyt kysymykset](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Lisätietoja sovellusten siirtämisestä käyttöympäristökohtaisesti](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Jos tarvitset apua ADAL-sovellusten käytössä, suosittelemme tarkistamaan kaikki sovellusten lähdekoodit ja tarvittaessa ottaa yhteyttä Internet-palveluntarjoajiin tai sovelluspalveluntarjoajiin. Microsoftin tukipalvelu voi myös tarjota sinulle luettelon kaikista vuokraajan ei-Microsoft ADAL -sovelluksista.

**AAD Graph -siirto**

Jos sovellus käyttää Azure AD Graph, noudata [ohjeitamme Azure AD Graph -sovellusten siirtämiseksi Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Siirron tarkistusluettelomme tarjoaa aloituspisteen.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Azure-sovelluksen rekisteröintiportaali näyttää, mitkä sovellukset käyttävät AAD Graphia. Suosittelemme, että tarkistat kaikki sovellusten lähdekoodit. Ota tarvittaessa yhteyttä internet-palveluntarjoajaan tai sovelluksen toimittajaan. Microsoft-tuki voi myös tarjota sinulle luettelon kaikista vuokraajasi AAD Graph käyttöomme.
3. Jotta sovellus voi käyttää Microsoft Graph:n tietoja, käyttäjän tai järjestelmänvalvojan on myönnettävä se oikeat käyttöoikeudet suostumusprosessin kautta. [Microsoft Graph -käyttöoikeusviittaus sisältää](https://docs.microsoft.com/graph/permissions-reference) microsoftin ohjelmointirajapintojen kuhunkin pääjoukkoon Graph liittyvät käyttöoikeudet. Artikkelissa on myös ohjeita käyttöoikeuksien käyttöön.
