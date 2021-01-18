---
title: SAML-assertions (Tokens)
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
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885213"
---
# <a name="saml-assertions-tokens"></a>SAML-assertions (Tokens)

1. SAML (Security Assertions Markup Language) -tunnukset ovat vaateiden XML-esityksiä. Oletusarvon mukaan SAML-tunnukset, joita Windows Communication Foundation (WCF) käyttää liittouissa suojausskenaarioissa, myönnetään tunnuksia. Lisätietoja on [saml-tunnusten ja -vaateiden tunnuksissa.](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)
2. Microsoftin tunnistetietoympäristö lähettää erilaisia suojaustunnuksia kunkin todennusvirran käsittelyssä. [SAML-tunnuksen väiteviittaus](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) kuvaa SAML 2.0 -tunnusten muotoa, suojausominaisuuksia ja sisältöä.
3. Noudata Microsoftin tunnistetietoympäristön [Määritettävissä](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) olevat tunnusten käyttöiät -kohdasta annettuja ohjeita, jotta ymmärrät, miten tunnusten elinkaari määritetään.
4. Noudata tässä artikkelissa kuvattuja [ohjeita Azure](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) AD SAML -tunnuksen salauksen määrittämiseen.
5. Azure AD:ssä voit määrittää varmenteen allekirjoitusasetukset ja varmenteen allekirjoitusalgoritmin. Lisätietoja on Azure Active Directoryn valikoimasovellusten [SAML-tunnuksen varmenteen lisäallekirjoitusvaihtoehdoissa.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)
