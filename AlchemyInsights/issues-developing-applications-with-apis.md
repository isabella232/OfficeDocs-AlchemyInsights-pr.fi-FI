---
title: Ohjelmointirajapintojen kanssa kehittyvien sovellusten ongelmat
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
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974618"
---
# <a name="issues-developing-applications-with-apis"></a>Sovellusten ohjelmointirajapintojen kehittämiseen liittyvät ongelmat

Jos haluat aloittaa Azure Active Directory Graph -ohjelmointirajapinnan käytön, tutustu [Azure AD Graph API:n pika-aloitusoppaaseen](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) tai tarkastele vuorovaikutteisia [Azure AD Graph -ohjelmointirajapinnan viitedokumentaatioita.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Azure Active Directory -todennuskirjaston (ADAL) ja Azure AD Graph API:n (AAD Graph) tuen päättyminen**

**30. kesäkuuta 2020** alkaen uusia ominaisuuksia ei enää lisätä ADAL:een ja Azure AD Graphiin. Teknisen tuen ja suojauspäivitysten tarjoaminen jatkuu, mutta ominaisuuspäivityksiä ei enää tarjota.

**30. kesäkuuta 2022** alkaen microsoft lopettaa ADAL: n ja Azure AD Graphin tuen, eikä se enää tarjoa teknistä tukea tai suojauspäivityksiä.

Sovellukset, jotka käyttävät ADAL:tä nykyisissä käyttöjärjestelmäversioissa, toimivat edelleen tämän ajan kuluttua, mutta eivät saa teknistä tukea tai suojauspäivityksiä.

Azure AD Graphia tämän jälkeen käyttävät sovellukset eivät ehkä enää saa vastauksia Azure AD Graph -päätepisteltä.

**ADAL-siirto**

Suosittelemme päivittämään [Microsoftin todentamiskirjastoon (MSAL),](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)jossa on uusimmat ominaisuudet ja suojauspäivitykset.

Jos käytät Microsoft-sovelluksia, tiedät, että Microsoft on parhaillaan muuttamassa sovelluksiaan MSAL-sovelluksiin tuen päättymiseen mennessä, jotta ne hyötyvät MSAL:n käynnissä olevista suojaus- ja ominaisuusparannuksista.

1. [Lue ADAL:n usein kysytyt kysymykset.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Lue lisää siitä, miten voit siirtää sovelluksia käyttöympäristökohtaisesti.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Jos tarvitset apua sen ymmärtämiseen, mitkä sovellukset käyttävät ADAL:tä, suosittelemme tarkistamaan kaikki sovellusten lähdekoodit ja tarvittaessa ottaa yhteyttä internet-palveluntarjoajiin tai sovellustarjoajiin. Microsoft-tuki voi myös tarjota sinulle luettelon kaikista vuokraajan ei-Microsoft ADAL -sovelluksista.

**AAD Graph -siirto**

Jos sovellus käyttää Azure AD Graphia, noudata ohjeita azure AD Graph -sovellusten [siirtämiseksi Microsoft Graphiin.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [Siirron tarkistusluettelomme tarjoaa aloituspisteen.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
1. Azure-sovelluksen rekisteröintiportaali näyttää, mitkä sovellukset käyttävät AAD Graphia. Suosittelemme, että tarkistat kaikki sovellusten lähdekoodit, ja ota tarvittaessa yhteyttä internet-palveluntarjoajiin tai sovelluspalveluntarjoajiin. Microsoft-tuki voi myös tarjota sinulle luettelon vuokraajan kaikista AAD Graph -käytöstä.
1. Jotta sovellus voi käyttää Microsoft Graphin tietoja, käyttäjän tai järjestelmänvalvojan on myönnettävä se oikeat käyttöoikeudet suostumusprosessin kautta. [Microsoft Graph -käyttöoikeusviittauksessa](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) luetellaan kuhunkin Microsoft Graph -ohjelmointirajapintojen pääjoukkoon liittyvät käyttöoikeudet. Artikkelissa on myös ohjeita käyttöoikeuksien käyttöön.
