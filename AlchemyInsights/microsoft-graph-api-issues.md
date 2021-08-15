---
title: Microsoft Graph-ohjelmointirajapinnan ongelmat
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
- "9004345"
- "7759"
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975890"
---
# <a name="microsoft-graph-api-issues"></a>Microsoft Graph-ohjelmointirajapinnan ongelmat

Tämä ohjeaihe voi koskea myös kehittäjiä, jotka käyttävät edelleen Azure AD:Graph ohjelmointirajapintaa. On kuitenkin erittäin suositeltavaa **käyttää** Microsoft Graph kaikissa hakemisto-, käyttäjätiedot- ja käytönhallintaskenaarioissa.

**Todennus- tai valtuutusongelmat**

- Jos sovellus  ei voi hankkia tunnuksia Microsoft Graph-puheluita varten, valitse Ongelma käyttöoikeustunnuksen **(todennuksen)** Microsoft Graph -luokassa, niin saat tarkempia ohjeita ja tukea tästä aiheesta.
- Jos sovellus saa **401-** tai 403-valtuutusvirheitä Microsoft Graph-puheluissa, valitse Käyttö estetty -virhe **(Valtuutus)** Microsoft Graph API -luokka, niin saat tarkempia ohjeita ja tukea tästä aiheesta.

**Haluan käyttää Microsoft Graph, mutta en tiedä, mistä aloittaa**

- [Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Yleistä Microsoft Graph:n käyttäjätietojen ja käytön hallinnasta](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Microsoft Graph -sovellusten rakentamisen aloittaminen](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – Microsoft Graph ohjelmointirajapintojen testaaminen vuokraajassa tai esittelytilaajassa

**Haluan käyttää Microsoft Graph, mutta tukeeko se tarvitsen v1.0-hakemiston ohjelmointirajapinnat?**

Microsoft Graph on suositeltu ohjelmointirajapinta hakemiston, käyttäjätietojen ja käytön hallintaan. Azure AD Graph:n ja Microsoft Graph:n mahdollisuuksien välillä on kuitenkin muutamia Graph. Tutustu seuraaviin artikkeleihin, joissa korostetaan ajan tasalla olevaa eroavaisuuksia, jotka auttavat valinnassasi:

- [Azure AD Graph:n ja Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD -ominaisuuden Graph Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD:n ja Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Ohjelmointirajapinta, johon soitan, ei toimi – missä voin tehdä enemmän testausta?**

**Microsoft Graph Explorer** – Testaa Microsoft Graph -ohjelmointirajapinnat vuokraajassa tai esittelytilaajassa  ja tutustu myös esimerkkikyselyihin Microsoft Graph Resurssienhallinnassa.

**Sovellukseni on liian hidas ja sitä myös niitetaan. Mitä parannuksia voin tehdä?**

Skenaariostasi riippuen käytettävissäsi on useita vaihtoehtoja, joilla voit tehdä sovelluksesta entistä tehokkaammin ja joissakin tapauksissa vähemmän altis palvelulle (jos puheluita on liikaa).

- [Microsoft Graph parhaat käytännöt](https://docs.microsoft.com/graph/best-practices-concept)
- [Siirtopyynnöt](https://docs.microsoft.com/graph/json-batching)
- [Muutosten jäljitäminen deltakyselyn avulla](https://docs.microsoft.com/graph/delta-query-overview)
- [Muutoksista ilmoittaminen webhooksien kautta](https://docs.microsoft.com/graph/webhooks)
- [Throttling guidance](https://docs.microsoft.com/graph/throttling)

**Mistä löydän lisätietoja virheistä ja tunnetuista ongelmista?**

- [Microsoft Graph virhevastaustiedot](https://docs.microsoft.com/graph/errors)
- [Microsoft Graph:n tunnetut ongelmat](https://docs.microsoft.com/graph/known-issues)

**Mistä voin tarkistaa palvelun käytettävyyden ja yhteyden tilan?**

Niiden taustalla olevien palvelujen käytettävyys ja yhteydet, joita voidaan käyttää Microsoft Graph voivat vaikuttaa Microsoft Graph.

- Jos Azure Active Directory palvelun kunto, tarkista Azure-tilasivulla lueteltujen suojaus- ja käyttäjätietopalvelujen [tila.](https://azure.microsoft.com/status/) 
- Jos Office Microsoft Graph-palvelua, tarkista palvelujen tila, joka on lueteltu Office palvelun kunto [-koontinäytössä.](https://portal.office.com/adminportal/home#/servicehealth)

Microsoft Graph-valtuutusvirheet voivat johtua useista eri ongelmista, joista suurin osa aiheuttaa 401- tai 403-virheen. Esimerkiksi seuraavat voivat johtaa valtuutusvirheisiin:

- Virheelliset [tunnusoston työnkulut](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Huonosti määritetyt [käyttöoikeuksien laajuudet](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- [puuttuminen](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***Azure Active Directory -todennuskirjaston (ADAL) ja Azure AD Graph -ohjelmointirajapinnan (AAD-Graph) tuen päättyminen***

**30. kesäkuuta 2020** alkaen uusia ominaisuuksia ei enää lisätä ADAL- ja Azure AD Graph. Tarjoamme jatkossakin teknistä tukea ja suojauspäivityksiä, mutta emme enää tarjoa ominaisuuspäivityksiä.

**30. kesäkuuta 2022** alkaen Microsoft lopettaa ADAL- ja Azure AD Graph ei enää tarjoa teknistä tukea tai suojauspäivityksiä.

Sovellukset, jotka käyttävät ADAL:tä olemassa olevissa käyttöjärjestelmäversioissa, toimivat edelleen tämän ajan kuluttua, mutta eivät saa *mitään teknistä tukea tai suojauspäivityksiä.*

Sovellukset, jotka käyttävät Azure AD Graph tämän ajan jälkeen, eivät ehkä enää saa vastauksia Azure AD Graph päätepisteltä.

**ADAL-siirto**

Suosittelemme päivittämistä [Microsoft todentamiskirjastoon (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), jossa on uusimmat ominaisuudet ja suojauspäivitykset.

Jos käytät Microsoft-sovelluksia, tiedät, että Microsoft on parhaillaan muuttamassa sovelluksiaan MSAL-sovelluksiin tuen päättymiseen mennessä, joten ne hyötyvät MSAL:n käynnissä olevista suojaus- ja ominaisuusparannuksista.

1. [Lue ADAL:ää koskevat usein kysytyt kysymykset](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Lisätietoja sovellusten siirtämisestä käyttöympäristökohtaisesti](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Jos tarvitset apua ADAL-sovellusten käytössä, suosittelemme tarkistamaan kaikki sovellusten lähdekoodit ja tarvittaessa ottaa yhteyttä Internet-palveluntarjoajiin tai sovelluspalveluntarjoajiin. Microsoftin tukipalvelu voi myös tarjota sinulle luettelon kaikista vuokraajan ei-Microsoft ADAL -sovelluksista.

**AAD Graph -siirto**

Jos sovellus käyttää Azure AD Graph, noudata [ohjeitamme Azure AD Graph -sovellusten siirtämiseksi Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Siirron tarkistusluettelo tarjoaa aloituspisteen](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Azure-sovelluksen rekisteröintiportaali näyttää, mitkä sovellukset käyttävät AAD Graphia. Suosittelemme, että tarkistat kaikki sovellusten lähdekoodit. Ota tarvittaessa yhteyttä internet-palveluntarjoajaan tai sovelluksen toimittajaan. Microsoft-tuki voi myös tarjota sinulle luettelon kaikista vuokraajasi AAD Graph käyttöomme.
3. Jotta sovellus voi käyttää Microsoft Graph:n tietoja, käyttäjän tai järjestelmänvalvojan on myönnettävä se oikeat käyttöoikeudet suostumusprosessin kautta. [Microsoft Graph -käyttöoikeusviittaus sisältää](https://docs.microsoft.com/graph/permissions-reference) microsoftin ohjelmointirajapintojen kuhunkin pääjoukkoon Graph liittyvät käyttöoikeudet. Artikkelissa on myös ohjeita käyttöoikeuksien käyttöön.
