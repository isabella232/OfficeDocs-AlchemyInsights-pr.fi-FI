---
title: Token Claims and Attributes -tunnuksiin liittyvät ongelmat
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035890"
---
# <a name="issues-with-token-claims-and-attributes"></a>Token Claims and Attributes -tunnuksiin liittyvät ongelmat

**Tunnusvaatimusten päivittäminen, määrittäminen tai poistaminen**

1. Käyttämällä Azure Active Directorya (Azure [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) AD) voit mukauttaa roolivaatimuksen väitetyyppiä vastaustunnuksessa, jonka saat, kun olet valtuuttanut sovelluksen.
2. Sovelluskehittäjät voivat määrittää Azure AD -sovelluksissaan valinnaisten vaateiden avulla, mitä tunnuksia sovellus haluaa käyttää. Lisätietoja on kohdassa [Sovelluksesi valinnaisten vaateiden tarjoaminen.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Määritä ryhmävaatimukset sovelluksille Azure Active Directoryn avulla.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)
4. Jos käytät saumatonta kertakirjaamista sovelluksessasi, tutustu saml-tunnuksessa yrityssovellusten [SAML-tunnusten](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)myöntäjän vaatimusten mukauttamiseen.

**Claims Attribute Mapping**

1. Lisätietoja väiteiden yhdistämiskäytännön määrittämisestä PowerShellin avulla on kohdassa Mukauta vuokraajan tietyn sovelluksen tunnuksiin jätettyjä vaateita [(esikatselu).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Hakemistorakenteen laajennusmääritteiden avulla voit tallentaa Azure Active Directoryyn lisätietoja käyttäjäobjekteihin ja muihin hakemisto-objekteihin, kuten ryhmiin, vuokraajatietoihin ja palvelun pääobjekteihin. Vain käyttäjäobjektien laajennusmääritteitä voidaan käyttää sovellusten vaateiden hakemiseksi. [Hakemistorakenteen laajennusmääritteiden](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) käyttäminen vaateissa kuvaa, miten käyttäjätiedot lähetetään sovelluksiin tunnuksen väiteissä hakemistorakenteen laajennusten määritteiden avulla.

Lisätietoja tunnuksen vaateista on kohdassa:

- [Käyttöoikeustietueita koskevat vaateet](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Vaateet id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Väite,](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) että käyttäjä voi odottaa Azure AD B2C:n myöntämia tunnustunnuksia ja käyttöoikeustunnuksia
- [SAML-tunnuksen väiteviittaus](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
