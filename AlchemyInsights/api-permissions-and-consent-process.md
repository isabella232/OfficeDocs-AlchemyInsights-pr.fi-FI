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
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932058"
---
# <a name="api-permissions-and-consent-process"></a>Ohjelmointirajapinnan käyttöoikeudet ja suostumusprosessi

Jotta sovellus voi käyttää Microsoft Graph:n tietoja, käyttäjän tai järjestelmänvalvojan on myönnettävä se oikeat käyttöoikeudet suostumusprosessin kautta. [Microsoft Graph -käyttöoikeusviittaus](https://docs.microsoft.com/graph/permissions-reference) sisältää microsoftin ohjelmointirajapintojen kuhunkin pääjoukkoon Graph liittyvät käyttöoikeudet. Artikkelissa on myös ohjeita käyttöoikeuksien käyttöön.

**Palvelun pääobjektin määritäminen tai päivittäminen**

- [Luo serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – tässä artikkelissa kerrotaan, miten voit luoda uuden servicePrincipal-objektin.
- [Luo Azure AD &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) -palvelun pääobjekti portaalissa – Tässä artikkelissa kerrotaan, miten voit luoda uuden Azure Active Directory (Azure AD) -sovelluksen ja palvelun pääobjektin, jota voidaan käyttää roolipohjaisen käytön ohjausobjektin kanssa.
- [Sovellukset & palvelun](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) pääobjektit Azure AD:ssä – Tässä artikkelissa kuvataan sovelluksen rekisteröinti, sovelluksen objektit ja palvelun pääobjektit Azure Active Directory:ssa: mitä ne ovat, miten niitä käytetään ja miten ne liittyvät toisiinsa.

**Sovelluksen rekisteröinnin lisääminen tai päivittäminen ja järjestelmänvalvojan suostumuksen asentaminen**

- [Luo sovelluksen rekisteröinti](https://docs.microsoft.com/graph/api/application-post-applications) – tässä artikkelissa kerrotaan, miten voit luoda uuden sovellusobjektin.
- [Sovelluksen rekisteröinnin päivittäminen – ohjelmointirajapinnan](https://docs.microsoft.com/graph/api/application-update) käyttöoikeudet – tässä artikkelissa kerrotaan, miten voit päivittää sovellusobjektin ominaisuudet.
- [Järjestelmänvalvojan suostumuksen](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) antaminen – Järjestelmänvalvojan suostumus ja suostumus edellyttävät yleisesti, että järjestelmänvalvoja antaa suostumuksen erikseen.
- [RBAC (beeta) –](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) roolien hallintasäilö yhdenmukaisille roolimääritteille ja roolimäärityksille Microsoft 365 RBAC-tarjoajille, jotka tukevat useita päämääriä ja useita scopeteja yhdessä roolimäärityksessä. Tämä eroaa *rbacApplication-resurssityypistä.* Microsoft Intune on esimerkki tällaisesta RBAC-palveluntarjoajasta. Intunen roolimäärityksessä voi olla pääobjektien matriisi ja laajuusryhmien matriisi. **Tämä on beetaversiota, mikä tarkoittaa, että sitä kehitety edelleen eikä sitä suositella käytettäväksi tuotantoon.**
