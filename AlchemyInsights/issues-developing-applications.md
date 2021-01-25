---
title: Sovellusten kehittämiseen liittyvät ongelmat
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974475"
---
# <a name="issues-developing-applications"></a>Sovellusten kehittämiseen liittyvät ongelmat

Seuraavissa artikkeleissa on tietoja Azure Active Directory (AD) -sovellusten rakentamiseen yleisimpiä ongelmia varten:

- [I am seeing trouble signing in to application(s) using Chrome browser only](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [En tiedä, miten voin muuttaa sovellukseni tunnusten elinkaaren oletusarvoja](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [En tiedä, miten sovelluksen suostumus toimii](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [En tiedä, miten voin myöntää käyttöoikeuksia sovellukseeni](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [En ymmärrä delegoidun ja sovelluksen käyttöoikeuksien välistä eroa](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Azure Active Directory -todennuskirjaston (ADAL) ja Azure AD Graph API:n (AAD Graph) tuen päättyminen** _

- 30. kesäkuuta 2020 alkaen Uusia ominaisuuksia ei enää lisätä Azure Active Directory -todennuskirjastoon (ADAL) ja Azure AD Graph API:een (AAD Graph). Teknisen tuen ja suojauspäivitysten tarjoaminen jatkuu, mutta ominaisuuspäivityksiä ei enää tarjota.

- 30. kesäkuuta 2022 alkaen ADAL: n ja AAD Graphin tuki päättyy, eikä se enää tarjoa teknistä tukea tai suojauspäivityksiä. Tämän ehdon vuoksi vaikutukset ovat seuraavat:

    - Sovellukset, jotka käyttävät ADAL:tä olemassa olevissa käyttöjärjestelmäversioissa, toimivat edelleen tämän ajan kuluttua, mutta eivät saa teknistä tukea tai suojauspäivityksiä.

    - AAD Graphia tämän jälkeen käyttävät sovellukset eivät ehkä enää saa vastauksia AAD Graph -päätepisteltä

_ *ADAL-siirto**

Jos käytät Microsoft-sovelluksia, suosittelemme päivittämään Microsoftin todennuskirjastoon (MSAL), jossa on uusimmat ominaisuudet ja suojauspäivitykset. Tämä suositus koskee Sitä, että Microsoft aloittaa sovellustensa MSAL-sovelluksiin siirtymisprosessin tuen päättymiseen mennessä. 

Microsoftin siirtyminen MSAL-sovelluksiin varmistaa, että sovellukset hyötyvät MSAL:n käynnissä olevista suojaus- ja ominaisuusparannuksista.

1. [ADAL:n usein kysytyt kysymykset](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Lisätietoja sovellusten siirtämisestä käyttöympäristökohtaisesti](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Jos tarvitset apua sen ymmärtämiseen, mitkä sovellukset käyttävät ADAL:tä, suosittelemme tarkistamaan kaikki sovellusten lähdekoodit ja ottaa tarvittaessa yhteyttä itsenäisten ohjelmistotoimittajien (ISV) tai sovellustoimittajien kanssa. Microsoft-tuki voi myös tarjota sinulle luettelon kaikista vuokraajan ei-Microsoft ADAL -sovelluksista.

**AAD Graph -siirto**

Jos sovellus käyttää AAD Graphia, noudata ohjeitamme AAD Graph -sovellusten siirtämiseksi Microsoft Graphiin:

1. [Siirron tarkistusluettelomme tarjoaa aloituspisteen.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
2. Azure-sovelluksen rekisteröintiportaali näyttää, mitkä sovellukset käyttävät AAD Graphia. Suosittelemme, että tarkistat kaikki sovellusten lähdekoodit ja ota tarvittaessa yhteyttä kaikkiin itsenäisten ohjelmistotoimittajien (ISV) tai sovellustoimittajien käyttöön. Microsoft-tuki voi myös antaa tietoja AAD Graphin käytöstä vuokraajassasi.







