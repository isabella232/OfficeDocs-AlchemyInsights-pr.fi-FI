---
title: SAML Assertions (Tokens)
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
- "9004341"
- "7753"
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109237"
---
# <a name="saml-assertions-tokens"></a>SAML Assertions (Tokens)

1. SAML (Security Assertions Markup Language) -tunnukset ovat vaateiden XML-esityksiä. OLETUSARVON MUKAAN SAML-tunnukset Windows Communication Foundation (WCF) -tunnuksia käytetään liittouissa suojausskenaarioissa. Lisätietoja on kohdassa [SAML-tunnukset ja -vaateet.](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)
2. The Microsoftin käyttäjätietoympäristö emits several types of security tokens in the processing of each authentication flow. [SAML-tunnuksen](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) väiteviitteissä kuvataan SAML 2.0 -tunnusten muoto, suojausominaisuudet ja sisältö.
3. Noudata tunnuksen [elinkaaren määritettävissä olevia](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) ohjeita Microsoftin käyttäjätietoympäristö tunnuksen elinkaaren määrittämiseen.
4. Tässä artikkelissa kuvattujen ohjeiden [avulla voit määrittää](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) Azure AD SAML -tunnuksen salauksen.
5. Azure AD:ssä voit määrittää varmenteen allekirjoitusasetukset ja varmenteen allekirjoitusalgoritmin. Lisätietoja on kohdassa SAML-tunnusten varmennekirjausasetusten lisäasetukset [valikoimasovelluksissa Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)
