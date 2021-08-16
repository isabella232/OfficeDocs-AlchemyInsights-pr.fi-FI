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
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013421"
---
# <a name="issues-developing-applications"></a>Sovellusten kehittämiseen liittyvät ongelmat

Jos haluat tehdä vianmäärityksen Azure Active Directory (AD) -sovelluksissa, tutustu seuraaviin artikkeleihin:

- [I am seeing trouble signing in to application(s) using Chrome browser only](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [En tiedä, miten voin muuttaa sovelluksen tunnusten elinkaaren oletusarvoja](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [En tiedä, miten sovelluksen suostumus toimii](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [En tiedä, miten voin myöntää käyttöoikeuksia sovellukselleni](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [En ymmärrä delegoidun käyttöoikeuksien ja sovelluksen käyttöoikeuksien välistä eroa](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Azure Active Directory -todennuskirjaston (ADAL) ja Azure AD Graph -ohjelmointirajapinnan (AAD-Graph) tuen päättyminen***

- 30. kesäkuuta 2020 alkaen Microsoft ei enää lisää uusia ominaisuuksia Azure Active Directory -todentamiskirjastoon (ADAL) ja Azure AD Graph API:iin (AAD Graph). Tarjoamme jatkossakin teknistä tukea ja suojauspäivityksiä, mutta emme enää tarjoa ominaisuuspäivityksiä.

- 30. kesäkuuta 2022 alkaen Microsoft lopettaa ADAL- ja AAD Graph -tuen, eikä Microsoft enää tarjoa teknistä tukea tai suojauspäivityksiä. Tämän ehdon vuoksi seuraavat vaikutukset ovat seuraavat:

    - Sovellukset, jotka käyttävät ADAL:tä olemassa olevissa käyttöjärjestelmäversioissa, toimivat edelleen tämän ajan kuluttua, mutta eivät saa teknistä tukea tai suojauspäivityksiä.

    - AAD-Graph tämän jälkeen eivät ehkä enää saa vastauksia AAD Graph päätepisteltä

**ADAL-siirto**

Jos käytät Microsoft-sovelluksia, suosittelemme päivittämään Microsoftin todentamiskirjastoon (MSAL), joka sisältää uusimmat ominaisuudet ja suojauspäivitykset. Tämä suositus koskee sitä, että Microsoft aloittaa sovellustensa siirtymisprosessin MSAL-sovelluksiin tuen päättymiseen mennessä. 

Microsoftin sovellussiirron MSAL-versioon varmistaa, että sovellukset hyötyvät MSAL:n jatkuvasta tietoturvasta ja ominaisuuksien parannuksista.

1. [Lue ADAL:ää koskevat usein kysytyt kysymykset](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Lisätietoja sovellusten siirtämisestä käyttöympäristökohtaisesti](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Jos tarvitset apua ADAL-sovellusten käytön ymmärtämiseen, suosittelemme tarkistamaan kaikki sovellusten lähdekoodit ja ottaa tarvittaessa yhteyttä itsenäisten ohjelmistotoimittajien (ISV) tai sovellustoimittajien kanssa. Microsoftin tukipalvelu voi myös tarjota sinulle luettelon kaikista vuokraajan ei-Microsoft ADAL -sovelluksista.

**AAD Graph -siirto**

Jos sovellus käyttää AAD-Graph, noudata ohjeitamme ja siirrä AAD Graph sovellukset Microsoft Graph:

1. [Siirron tarkistusluettelo tarjoaa aloituspisteen](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Azure-sovelluksen rekisteröintiportaali näyttää, mitkä sovellukset käyttävät AAD Graphia. Suosittelemme, että tarkistat kaikki sovellusten lähdekoodit ja ota tarvittaessa yhteyttä itsenäisten ohjelmistotoimittajien (ISV) tai sovellustoimittajien kanssa. Microsoft-tuki voi myös antaa sinulle tietoja AAD Graph käytöstä vuokraajassasi.







