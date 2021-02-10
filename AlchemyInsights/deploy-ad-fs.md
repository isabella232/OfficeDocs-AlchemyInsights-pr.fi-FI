---
title: AD FS:n käyttöönotto
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
- "1300012"
- "7420"
ms.openlocfilehash: a304504f7483036884878639dfa6ebfc3cdfcac8
ms.sourcegitcommit: 05a9dd3121c21322dc9ddec4c2eec548cafd5a43
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177548"
---
# <a name="deploy-ad-fs"></a><span data-ttu-id="79dd8-102">AD FS:n käyttöönotto</span><span class="sxs-lookup"><span data-stu-id="79dd8-102">Deploy AD FS</span></span>

<span data-ttu-id="79dd8-103">Active Directory Federation Services (AD FS) -käyttöönotto todentaa käyttäjät Office 365 -palvelujen käyttäjille paikallisen infrastruktuurin avulla.</span><span class="sxs-lookup"><span data-stu-id="79dd8-103">An Active Directory Federation Services (AD FS) deployment uses your on-premises infrastructure to authenticate users for ‎Office 365 services.</span></span> <span data-ttu-id="79dd8-104">Kun käytät liitettyä kirjautumista, voit antaa käyttäjien kirjautua Office 365 -palveluihin ja -ohjelmistoihin palveluna (SAAS), jotka on integroitu Azure Active Directoryyn (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="79dd8-104">With federated sign-in, you can enable users to sign in to Office 365 services and Software as a Service (SAAS) applications that are integrated with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="79dd8-105">Liittoutettu kirjautuminen todentaa käyttäjät paikalliseen Active Directoryyn AD FS:n kautta.</span><span class="sxs-lookup"><span data-stu-id="79dd8-105">Federated sign-in authenticates users against your on-premises Active Directory via AD FS.</span></span> <span data-ttu-id="79dd8-106">Yritysverkossa käyttäjien ei myöskään tarvitse antaa salasanojaan uudelleen.</span><span class="sxs-lookup"><span data-stu-id="79dd8-106">Also, while on the corporate network, users won't be required to reenter their passwords.</span></span>

<span data-ttu-id="79dd8-107">AD FS -käyttöönottoneuvoja antaa vaiheittaiset ohjeet paikallisen [AD FS](https://go.microsoft.com/fwlink/?linkid=2071178) -infrastruktuurin käyttöönottoon, joka todentaa microsoft 365- ja Office 365 -palvelujen käyttäjät.</span><span class="sxs-lookup"><span data-stu-id="79dd8-107">The [AD FS deployment advisor](https://go.microsoft.com/fwlink/?linkid=2071178) provides you with step-by-step guidance on deploying an on-premises AD FS infrastructure that authenticates users for Microsoft 365 and Office 365 services.</span></span> <span data-ttu-id="79dd8-108">Tämän oppaan avulla organisaatiosi voi tarkastella AD FS:n osia ja vaatimuksia, hankkia ja asentaa käyttöönottoon tarvittavia SSL-varmenteita sekä asentaa vaaditun verkkosovelluksen välityspalvelimen.</span><span class="sxs-lookup"><span data-stu-id="79dd8-108">With this guide, your organization can review AD FS components and requirements, acquire and install SSL certificates that are necessary for deployment, and install a required web application proxy server.</span></span>
