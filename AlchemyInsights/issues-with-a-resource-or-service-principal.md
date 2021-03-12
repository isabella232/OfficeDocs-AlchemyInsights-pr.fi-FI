---
title: Resurssin tai palvelun pääobjektiin liittyvät ongelmat
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
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/28/2021
ms.locfileid: "50713662"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Resurssin tai palvelun pääobjektiin liittyvät ongelmat

1. Jos olet juuri aloittamassa, Sovellus- ja palvelun pääobjektit Azure Active Directoryssa kuvaavat [Azure Active Directoryn](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) sovellusten rekisteröintiä, sovellusobjekteja ja palvelun pääobjekteja: mitä ne ovat, miten niitä käytetään ja miten ne liittyvät toisiinsa. Usean vuokraajan esimerkkiskenaario esitetään myös havainnollistamaan sovelluksen sovellusobjektin ja vastaavien palvelun pääobjektien välistä suhdetta.
2. Saat lisätietoja sovellusten ja palvelun pääobjektien välisistä suhteista lukemalla sovelluksia ja palvelun [pääobjekteja Azure Active Directoryssa.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. [Ohjeet:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) Portaalin avulla voit luoda Azure AD -sovelluksen ja -palvelun pääobjektin, joilla voi käyttää resursseja, näyttää, miten voit luoda uuden Azure Active Directory (Azure AD) -sovelluksen ja palvelun pääobjektin, jota voidaan käyttää roolipohjaisessa käyttöoikeusohjausobjektissa.
4. Palvelun [päärajapinnan](https://docs.microsoft.com/graph/api/resources/serviceprincipal)avulla voit ohjelmallisesti hallita sovellusten esiintymät ja hallita, mitä sovellus voi tehdä vuokraajassasi.
5. [servicePrincipal-resurssityyppi](https://docs.microsoft.com/graph/api/resources/serviceprincipal) näyttää kaikki servicePrincipal-resurssityypin ominaisuudet ja menetelmät.
6. [Azure AD Graphin ja Microsoft Graphin](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) väliset resurssityyppierot korostuvat Azure AD Graphin ja Microsoft Graphin resurssien välisissä eroissa. Se näyttää resurssit, joiden nimi on eri tai jotka eivät ole käytettävissä. siinä korostetaan myös Microsoft Graphin beetaversiossa käytettävissä olevia resursseja, mutta ei v1.0-versiota.

**Vieraskäyttäjiin liittyvät ongelmat**

- [Pika-aloitus:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Vieraskäyttäjien lisääminen hakemistoon Azure-portaalissa näyttää, miten voit lisätä uuden vieraskäyttäjän Azure AD -hakemistoon Azure-portaalin kautta, lähettää kutsun ja nähdä, miltä vieraskäyttäjän kutsun lunastusprosessi näyttää.
- [Opetusohjelma: Käyttäjien työnkulkujen luominen Azure Active Directory B2C:ssä](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) näyttää, miten voit luoda joitakin suositeltuja käyttäjävirtoja Azure-portaalin avulla. Jos etsit tietoja siitä, miten voit määrittää resurssin omistajan salasanatunnukset (ROPC) sovelluksessa, katso lisätietoja resurssien omistajan salasanan tunnistetietojen työnkulun määrittämisestä Azure AD B2C:ssä.
