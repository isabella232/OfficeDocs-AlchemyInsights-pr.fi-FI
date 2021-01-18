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
# <a name="saml-assertions-tokens"></a><span data-ttu-id="efe8f-102">SAML-assertions (Tokens)</span><span class="sxs-lookup"><span data-stu-id="efe8f-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="efe8f-103">SAML (Security Assertions Markup Language) -tunnukset ovat vaateiden XML-esityksiä.</span><span class="sxs-lookup"><span data-stu-id="efe8f-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="efe8f-104">Oletusarvon mukaan SAML-tunnukset, joita Windows Communication Foundation (WCF) käyttää liittouissa suojausskenaarioissa, myönnetään tunnuksia.</span><span class="sxs-lookup"><span data-stu-id="efe8f-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="efe8f-105">Lisätietoja on [saml-tunnusten ja -vaateiden tunnuksissa.](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)</span><span class="sxs-lookup"><span data-stu-id="efe8f-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="efe8f-106">Microsoftin tunnistetietoympäristö lähettää erilaisia suojaustunnuksia kunkin todennusvirran käsittelyssä.</span><span class="sxs-lookup"><span data-stu-id="efe8f-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="efe8f-107">[SAML-tunnuksen väiteviittaus](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) kuvaa SAML 2.0 -tunnusten muotoa, suojausominaisuuksia ja sisältöä.</span><span class="sxs-lookup"><span data-stu-id="efe8f-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="efe8f-108">Noudata Microsoftin tunnistetietoympäristön [Määritettävissä](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) olevat tunnusten käyttöiät -kohdasta annettuja ohjeita, jotta ymmärrät, miten tunnusten elinkaari määritetään.</span><span class="sxs-lookup"><span data-stu-id="efe8f-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="efe8f-109">Noudata tässä artikkelissa kuvattuja [ohjeita Azure](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) AD SAML -tunnuksen salauksen määrittämiseen.</span><span class="sxs-lookup"><span data-stu-id="efe8f-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="efe8f-110">Azure AD:ssä voit määrittää varmenteen allekirjoitusasetukset ja varmenteen allekirjoitusalgoritmin.</span><span class="sxs-lookup"><span data-stu-id="efe8f-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="efe8f-111">Lisätietoja on Azure Active Directoryn valikoimasovellusten [SAML-tunnuksen varmenteen lisäallekirjoitusvaihtoehdoissa.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)</span><span class="sxs-lookup"><span data-stu-id="efe8f-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
