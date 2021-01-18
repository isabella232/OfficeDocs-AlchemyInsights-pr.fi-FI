---
title: Sovelluksen välityspalvelimen määritys
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885131"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="fba41-102">Sovelluksen välityspalvelimen määritys</span><span class="sxs-lookup"><span data-stu-id="fba41-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="fba41-103">Lisätietoja sovellusten välityspalvelimen sovelluksen määrittämisestä Azure AD:ssä, jotta paikallissovellukset voidaan näyttää pilvipalvelussa, on kohdassa Sovelluksen [välityspalvelinsovelluksen määrittäminen.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)</span><span class="sxs-lookup"><span data-stu-id="fba41-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="fba41-104">Kertakirjautumisen avulla käyttäjät voivat käyttää sovellusta todentamatta useita kertoja.</span><span class="sxs-lookup"><span data-stu-id="fba41-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="fba41-105">Sen avulla yksittäinen todennus voidaan suorittaa pilvessä Azure Active Directorya vastaan ja sen avulla palvelu tai yhdistin voi tekeytyä käyttäjän sovelluksesta syntyviin muihin todennushaasteisiin.</span><span class="sxs-lookup"><span data-stu-id="fba41-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="fba41-106">Lisätietoja on kohdassa [Kertakirjauksesi määrittäminen sovelluksen välityspalvelinsovellukseen.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)</span><span class="sxs-lookup"><span data-stu-id="fba41-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="fba41-107">Tämän [artikkelin avulla voit](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) tehdä vianmäärityksen yleisiin ongelmiin, joita ihmiset kohtaavat luotaessa uutta sovelluksen välityspalvelinsovellusta.</span><span class="sxs-lookup"><span data-stu-id="fba41-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="fba41-108">Jos sinulla on ongelmia sovelluksesi taustatodentamisen määrittämisessä, sinun on ehkä [vianmääritystä Kerberosin](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) rajoitettuja delegointimäärityksiä sovelluksen välityspalvelinta varten tai seurattava ohjeita sovelluksen määrittämiseen [PingAccessilla](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) ongelman ratkaisemiseksi.</span><span class="sxs-lookup"><span data-stu-id="fba41-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
