---
title: Microsoft Graphin ohjelmointirajapinnan ongelmat
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
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/29/2021
ms.locfileid: "50713702"
---
# <a name="microsoft-graph-api-issues"></a>Microsoft Graphin ohjelmointirajapinnan ongelmat

Tämä ohjeaihe voi koskea myös kehittäjiä, jotka käyttävät edelleen Azure AD Graph -ohjelmointirajapintaa. On kuitenkin erittäin **suositeltavaa,** että käytät Microsoft Graphia kaikissa hakemisto-, käyttäjätiedot- ja käytönhallintaskenaarioissa.

**Todennus- tai valtuutusongelmat**

- Jos sovellus  ei voi hankkia tunnuksia Microsoft Graph -kutsumista varten, valitse Ongelma, kun saat käyttöoikeustietueen **(todennuksen)** Microsoft Graph -luokan, niin saat tarkempia ohjeita ja tukea tästä aiheesta.
- Jos sovellus saa **401-** tai 403-valtuutusvirheitä Microsoft Graphia kutsuttaessa, valitse Hae käyttö estetty **-virhe (Valtuutus)** Microsoft Graph API -luokka, niin saat tarkempia ohjeita ja tukea tästä aiheesta.

**Haluan käyttää Microsoft Graphia, mutta en tiedä, mistä aloittaa**

- [Yleistä Microsoft Graphista](https://docs.microsoft.com/graph/overview)
- [Yleistä käyttäjätietojen ja käytön hallinnasta Microsoft Graphissa](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Microsoft Graph -sovellusten rakentamisen aloittaminen](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – Microsoft Graph -ohjelmointirajapintojen testaaminen vuokraajassa tai esittely vuokraajassa

**Haluan käyttää Microsoft Graphia, mutta tukeeko se tarvitsemii v1.0-hakemistorajapintojen käyttöä?**

Microsoft Graph on hakemiston, käyttäjätietojen ja käytön hallinnan suositeltu ohjelmointirajapinta. Azure AD Graphin ja Microsoft Graphin välillä on kuitenkin vielä muutamia aukkoja. Tutustu seuraaviin artikkeleihin, joissa korostetaan uusimpia eroja, jotka auttavat valitsemaan:

- [Resurssityyppierot Azure AD Graphin ja Microsoft Graphin välillä](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD Graphin ja Microsoft Graphin ominaisuuden erot](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD:n ja Microsoft Graphin väliset menetelmäerot](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Ohjelmointirajapinta, johon soitan, ei toimi – missä voin tehdä enemmän testausta?**

**Microsoft Graph Explorer** – Testaa Microsoft Graph -ohjelmointirajapinnat vuokraajassa  tai esittely vuokraajassa ja tutustu myös mallikyselyihin Microsoft Graph Explorerissa.

**Sovellukseni on liian hidas ja sitä myös käytetään kursivassa. Mitä parannuksia voin tehdä?**

Skenaariostasi riippuen käytettävissäsi on useita vaihtoehtoja, joilla voit tehdä sovelluksesta entistä tehokkaammin ja joissakin tapauksissa vähemmän altis palvelun utelle (kun puheluita on liikaa).

- [Microsoft Graphin parhaat käytännöt](https://docs.microsoft.com/graph/best-practices-concept)
- [Siirtopyynnöt](https://docs.microsoft.com/graph/json-batching)
- [Muutosten jäljitäminen deltakyselyn avulla](https://docs.microsoft.com/graph/delta-query-overview)
- [Saa ilmoituksia muutoksista verkko-osien kautta](https://docs.microsoft.com/graph/webhooks)
- [Kursimisohjeet](https://docs.microsoft.com/graph/throttling)

**Mistä löydän lisätietoja virheistä ja tunnetuista ongelmista?**

- [Microsoft Graphin virhevastaustiedot](https://docs.microsoft.com/graph/errors)
- [Microsoft Graphin tunnetut ongelmat](https://docs.microsoft.com/graph/known-issues)

**Mistä voin tarkistaa palvelun käytettävyyden ja yhteyden tilan?**

Niiden taustalla olevien palvelujen käytettävyys ja yhteydet, joita voidaan käyttää Microsoft Graphin kautta, voivat vaikuttaa Microsoft Graphin yleiseen käytettävuuteen ja suorituskykyyn.

- Tarkista Azure Active Directory -palvelun kuntoa varten Azure-tilasivulla lueteltujen **suojaus-** ja [käyttäjätietopalvelujen tila.](https://azure.microsoft.com/status/)
- Tarkista Microsoft Graphiin osallistuneet Office-palvelut Office Service Health -koontinäytössä lueteltujen [palvelujen tila.](https://portal.office.com/adminportal/home#/servicehealth)

Microsoft Graphin valtuutusvirheet voivat johtua useista eri ongelmista, joista useimmat luovat 401- tai 403-virheen. Esimerkiksi seuraavat voivat johtaa valtuutusvirheisiin:

- Virheelliset [tunnusoston työnkulut](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Huonosti määritetyt [käyttöoikeuksien laajuudet](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- [puuttuminen](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Azure Active Directory -todentamiskirjaston (ADAL) ja Azure AD Graph API:n (AAD Graph) tuen päättyminen_* _

_*30. kesäkuuta 2020** alkaen uusia ominaisuuksia ei enää lisätä ADAL:een ja Azure AD Graphiin. Tarjoamme jatkossakin teknistä tukea ja suojauspäivityksiä, mutta emme enää tarjoa ominaisuuspäivityksiä.

**30. kesäkuuta 2022** alkaen microsoft lopettaa ADAL: n ja Azure AD Graphin tuen, eikä se enää tarjoa teknistä tukea tai suojauspäivityksiä.

Sovellukset, jotka käyttävät ADAL:tä nykyisissä käyttöjärjestelmäversioissa, toimivat edelleen tämän ajan kuluttua, mutta eivät saa *mitään teknistä tukea tai suojauspäivityksiä.*

Azure AD Graphia tämän jälkeen käyttävät sovellukset eivät ehkä enää saa vastauksia Azure AD Graph -päätepisteltä.

**ADAL-siirto**

Suosittelemme päivittämistä [Microsoft todentamiskirjastoon (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), jossa on uusimmat ominaisuudet ja suojauspäivitykset.

Jos käytät Microsoft-sovelluksia, tiedät, että Microsoft on parhaillaan muuttamassa sovelluksiaan MSAL-sovelluksiin tuen päättymiseen mennessä, jotta ne hyötyvät MSAL:n käynnissä olevista suojaus- ja ominaisuusparannuksista.

1. [Lue ADAL:ää koskevat usein kysytyt kysymykset](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Lisätietoja sovellusten siirtämisestä käyttöympäristökohtaisesti](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Jos tarvitset apua sen ymmärtämiseen, mitkä sovellukset käyttävät ADAL:tä, suosittelemme tarkistamaan kaikki sovellusten lähdekoodit ja tarvittaessa ottaa yhteyttä internet-palveluntarjoajiin tai sovellustarjoajiin. Microsoftin tukipalvelu voi myös tarjota sinulle luettelon kaikista vuokraajan ei-Microsoft ADAL -sovelluksista.

**AAD Graph -siirto**

Jos sovellus käyttää Azure AD Graphia, noudata ohjeita azure AD Graph -sovellusten [siirtämiseksi Microsoft Graphiin.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Siirron tarkistusluettelo tarjoaa aloituspisteen](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Azure-sovelluksen rekisteröintiportaali näyttää, mitkä sovellukset käyttävät AAD Graphia. Suosittelemme, että tarkistat kaikki sovellusten lähdekoodit. Ota tarvittaessa yhteyttä internet-palveluntarjoajaan tai sovelluksen toimittajaan. Microsoft-tuki voi myös tarjota sinulle luettelon vuokraajan kaikista AAD Graph -käytöstä.
3. Jotta sovellus voi käyttää Microsoft Graphin tietoja, käyttäjän tai järjestelmänvalvojan on myönnettävä se oikeat käyttöoikeudet suostumusprosessin kautta. [Microsoft Graph -käyttöoikeusviittauksessa](https://docs.microsoft.com/graph/permissions-reference) luetellaan kuhunkin Microsoft Graph -ohjelmointirajapintojen pääjoukkoon liittyvät käyttöoikeudet. Artikkelissa on myös ohjeita käyttöoikeuksien käyttöön.
