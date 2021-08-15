---
title: Sovellusten kehittämiseen ohjelmointirajapintojen avulla liittyvät ongelmat
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013457"
---
# <a name="issues-developing-applications-with-apis"></a>Sovellusten kehittämiseen ohjelmointirajapintojen avulla liittyvät ongelmat

Jos haluat aloittaa Azure Active Directory Graph-ohjelmointirajapinnan käytön, tutustu [Azure AD Graph API:n pika-aloitusoppaaseen](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) tai tarkastele vuorovaikutteisia [Azure AD Graph -ohjelmointirajapinnan viitedokumentaatiota.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Azure Active Directory -todennuskirjaston (ADAL) ja Azure AD Graph -ohjelmointirajapinnan (AAD-Graph) tuen päättyminen**

**30. kesäkuuta 2020** alkaen uusia ominaisuuksia ei enää lisätä ADAL- ja Azure AD Graph. Tarjoamme jatkossakin teknistä tukea ja suojauspäivityksiä, mutta emme enää tarjoa ominaisuuspäivityksiä.

**30. kesäkuuta 2022** alkaen Microsoft lopettaa ADAL- ja Azure AD Graph ei enää tarjoa teknistä tukea tai suojauspäivityksiä.

Sovellukset, jotka käyttävät ADAL:tä olemassa olevissa käyttöjärjestelmäversioissa, toimivat edelleen tämän ajan kuluttua, mutta eivät saa teknistä tukea tai suojauspäivityksiä.

Sovellukset, jotka käyttävät Azure AD Graph tämän ajan jälkeen, eivät ehkä enää saa vastauksia Azure AD Graph päätepisteltä.

**ADAL-siirto**

Suosittelemme päivittämistä [Microsoft todentamiskirjastoon (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), jossa on uusimmat ominaisuudet ja suojauspäivitykset.

Jos käytät Microsoft-sovelluksia, tiedät, että Microsoft on parhaillaan muuttamassa sovelluksiaan MSAL-tiliin tuen päättymiseen mennessä ja varmistaen, että ne hyötyvät MSAL:n meneillään olevista suojaus- ja ominaisuusparannuksista.

1. [Lue ADAL:n usein kysytyt kysymykset.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Lue, miten voit siirtää sovelluksia käyttöympäristökohtaisesti.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Jos tarvitset apua ADAL-sovellusten käytössä, suosittelemme tarkistamaan kaikki sovellusten lähdekoodit ja tarvittaessa ottaa yhteyttä Internet-palveluntarjoajiin tai sovelluspalveluntarjoajiin. Microsoftin tukipalvelu voi myös tarjota sinulle luettelon kaikista vuokraajan ei-Microsoft ADAL -sovelluksista.

**AAD Graph -siirto**

Jos sovellus käyttää Azure AD Graph, noudata [ohjeitamme Azure AD Graph -sovellusten siirtämiseksi Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [Siirron tarkistusluettelo tarjoaa aloituspisteen](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Azure-sovelluksen rekisteröintiportaali näyttää, mitkä sovellukset käyttävät AAD Graphia. Suosittelemme, että tarkistat kaikki sovellusten lähdekoodit. Ota tarvittaessa yhteyttä internet-palveluntarjoajaan tai sovelluksen toimittajaan. Microsoft-tuki voi myös tarjota sinulle luettelon kaikista vuokraajasi AAD Graph käyttöomme.
1. Jotta sovellus voi käyttää Microsoft Graph:n tietoja, käyttäjän tai järjestelmänvalvojan on myönnettävä se oikeat käyttöoikeudet suostumusprosessin kautta. [Microsoft Graph -käyttöoikeusviittaus sisältää](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) microsoftin ohjelmointirajapintojen kuhunkin pääjoukkoon Graph liittyvät käyttöoikeudet. Artikkelissa on myös ohjeita käyttöoikeuksien käyttöön.
