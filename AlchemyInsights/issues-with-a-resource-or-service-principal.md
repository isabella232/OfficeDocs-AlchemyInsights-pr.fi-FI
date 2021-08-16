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
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028073"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Resurssin tai palvelun pääobjektiin liittyvät ongelmat

1. Jos olet vasta aloittamassa, [Azure Active Directory:n](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) sovellus- ja palvelun pääobjektit kuvaavat sovelluksen rekisteröintiä, sovelluksen objekteja ja palvelun pääobjekteja Azure Active Directory:ssa: mitä ne ovat, miten niitä käytetään ja miten ne liittyvät toisiinsa. Usean vuokraajan esimerkkiskenaario esitetään myös kuvaamaan sovelluksen sovellusobjektin ja vastaavien palvelun pääobjektien välistä suhdetta.
2. Saat lisätietoja sovellusten ja palvelun pääobjektien välisistä suhteista lukemalla sovelluksia ja palvelun [pääobjekteja Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. [Ohjeet:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) Portaalin avulla voit luoda Azure AD -sovelluksen ja -palvelun pääobjektin, joka voi käyttää resursseja, näyttää, miten voit luoda uuden Azure Active Directory (Azure AD) -sovelluksen ja palvelun pääobjektin, jota voidaan käyttää roolipohjaisen käytön ohjausobjektin kanssa.
4. Palvelun [päärajapinnan](https://docs.microsoft.com/graph/api/resources/serviceprincipal)avulla voit hallita sovellusten esiintymät ohjelmallisesti ja määrittää, mitä sovellus voi tehdä vuokraajassasi.
5. [servicePrincipal-resurssityyppi](https://docs.microsoft.com/graph/api/resources/serviceprincipal) näyttää kaikki servicePrincipal-resurssityypin ominaisuudet ja menetelmät.
6. [Azure AD Graph:n ja Microsoft Graph:n](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) väliset resurssilajierot korostuvat Azure AD Graph Microsoft Graph resurssien välillä. Se näyttää resurssit, joiden nimi on eri tai jotka eivät ole käytettävissä. siinä korostetaan myös Microsoft Graph:n beetaversiossa saatavilla olevia resursseja, mutta ei v1.0-versiota.

**Vieraskäyttäjiin liittyvät ongelmat**

- [Pika-aloitus:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Vieraskäyttäjien lisääminen hakemistoon Azure-portaalissa näyttää, miten voit lisätä uuden vieraskäyttäjän Azure AD -hakemistoon Azure-portaalin kautta, lähettää kutsun ja nähdä, miltä vieraskäyttäjän kutsun lunastusprosessi näyttää.
- [Opetusohjelma: Käyttäjien työnkulkujen luominen Azure Active Directory B2C:ssä](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) näyttää, miten voit luoda joitakin suositeltuja käyttäjävirtoja Azure-portaalin avulla. Jos etsit tietoja resurssin omistajan salasanan tunnistetietojen (ROPC) määrittämisestä sovelluksessa, katso resurssin omistajan salasanan tunnistetietojen työnkulun määrittäminen Azure AD B2C:ssä.
