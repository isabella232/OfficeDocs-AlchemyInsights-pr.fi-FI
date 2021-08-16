---
title: Tunnusväitteiden ja -määritteiden ongelmat
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
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012881"
---
# <a name="issues-with-token-claims-and-attributes"></a>Tunnusväitteiden ja -määritteiden ongelmat

**Tunnusvaatimusten päivittäminen, määrittäminen tai poistaminen**

1. Käyttämällä Azure Active Directory (Azure AD) -ratkaisua voit mukauttaa roolivaatimuksen väitetyyppiä vastaustietueissa, jotka saat sovelluksen valtuuttamisen jälkeen. [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)
2. Sovelluskehittäjät voivat azure AD -sovellustensa valinnaisten vaateiden avulla määrittää, mitä vaateita he haluavat sovellukseensa lähetetyissä tunnuksissa. Lisätietoja on kohdassa [Valinnaisten vaateiden tarjoaminen sovellukseen.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Määritä ryhmävaatimukset sovelluksille, joissa on Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)
4. Jos käytät sovelluksessa saumatonta kertakirjaamista, katso saml-tunnuksessa myönnettyjen [vaateiden mukauttaminen yrityssovelluksissa.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Claims Attribute Mapping**

1. Lisätietoja väitemäärityskäytännön määrittämisestä PowerShellin avulla on kohdassa Mukauta vuokraajan tietyn sovelluksen tunnuksissa olevia vaateita [(esikatselu).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Hakemistorakenteen laajennusten määritteiden avulla voit tallentaa lisätietoja käyttäjäobjekteihin Azure Active Directory muihin hakemisto-objekteihin, kuten ryhmiin, vuokraajatietoihin ja palvelun päänimiin. Vain käyttäjäobjektien tunnistemääritteitä voidaan käyttää sovellusten vaateiden hakemiseksi. [Hakemistorakenteen laajennusmääritteiden](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) käyttäminen vaatimuksista kuvaa, miten hakemistorakenteen alanumeromääritteitä käytetään käyttäjien tietojen lähettämiseen sovelluksiin tunnuksen vaateissa.

Lisätietoja tunnusvaatimuksista on kohdassa:

- [Vaateet käyttöoikeustietueissa](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Vaateet id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Väite,](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) että käyttäjä voi odottaa Azure AD B2C:n myöntäjän tunnustietueissa ja käyttöoikeustietueissa
- [SAML-tunnuksen väiteviite](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
