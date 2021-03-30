---
title: Ohjelmointirajapinnan käyttöoikeudet ja suostumusprosessi
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404504"
---
# <a name="api-permissions-and-consent-process"></a>Ohjelmointirajapinnan käyttöoikeudet ja suostumusprosessi

Jotta sovellus voi käyttää Microsoft Graphin tietoja, käyttäjän tai järjestelmänvalvojan on myönnettävä se oikeat käyttöoikeudet suostumusprosessin kautta. [Microsoft Graph -käyttöoikeusviittaus](https://docs.microsoft.com/graph/permissions-reference) sisältää kuhunkin Microsoft Graph -ohjelmointirajapintojen pääjoukkoon liittyvät käyttöoikeudet. Artikkelissa on myös ohjeita käyttöoikeuksien käyttöön.

**Palvelun pääobjektin määritäminen tai päivittäminen**

- [Luo serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – tässä artikkelissa kerrotaan, miten voit luoda uuden servicePrincipal-objektin.
- [Luo Azure AD -&](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) palvelun päärooli portaaliin – Tässä artikkelissa kerrotaan, miten voit luoda uuden Azure Active Directory (Azure AD) -sovelluksen ja palvelun pääobjektin, jota voidaan käyttää roolipohjaisessa käyttöoikeusohjausobjektissa.
- [Sovellukset & Azure AD:n](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) palvelun päätoiminnuksissa – Tässä artikkelissa kuvataan sovellusten rekisteröinti, sovellusobjektit ja palvelun pääobjektit Azure Active Directoryssa: mitä ne ovat, miten niitä käytetään ja miten ne liittyvät toisiinsa.

**Sovelluksen rekisteröinnin lisääminen tai päivittäminen ja järjestelmänvalvojan suostumuksen tarjoaminen**

- [Luo sovelluksen rekisteröinti](https://docs.microsoft.com/graph/api/application-post-applications) – tässä artikkelissa kerrotaan, miten voit luoda uuden sovellusobjektin.
- [Sovelluksen rekisteröinnin päivittäminen – ohjelmointirajapinnan](https://docs.microsoft.com/graph/api/application-update) käyttöoikeudet – Tässä artikkelissa kerrotaan, miten voit päivittää sovellusobjektin ominaisuuksia.
- [Anna järjestelmänvalvojan suostumus](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) – Järjestelmänvalvojan suostumus ja suostumus edellyttävät yleensä, että järjestelmänvalvoja antaa nimenomaisesti suostumuksen.
- [RBAC (beeta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – Roolien hallintasäilö microsoft 365:n RBAC-tarjoajille, jotka tukevat useita päämääriä ja useita vaikutusalueiden määriä yhdessä roolimäärityksessä. Tämä eroaa *rbacApplication-resurssityypistä.* Microsoft Intune on esimerkki tällaisesta RBAC-palveluntarjoajasta. Intunen roolimäärityksessä voi olla pääryhmien matriisi ja alueryhmien matriisi. **Tämä on beetaversiota, mikä tarkoittaa, että se on edelleen kehitysvaiheessa eikä sitä suositella käytettäväksi tuotannossa.**
