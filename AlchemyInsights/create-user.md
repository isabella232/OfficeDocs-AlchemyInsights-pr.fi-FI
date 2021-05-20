---
title: Luo käyttäjä
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569720"
---
# <a name="create-user"></a><span data-ttu-id="89282-102">Luo käyttäjä</span><span class="sxs-lookup"><span data-stu-id="89282-102">Create user</span></span>

<span data-ttu-id="89282-103">**ILMOITUS:**</span><span class="sxs-lookup"><span data-stu-id="89282-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="89282-104">[WebView-kirjautumistuen peruuttaminen Googlesta 4. tammikuuta 2021 alkaen.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support)</span><span class="sxs-lookup"><span data-stu-id="89282-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="89282-105">Testaa, vaikuttaako Googlen yhteensopivuuden testaamista koskevat ohjeet [sovelluksiin.](https://go.microsoft.com/fwlink/?linkid=2157323)</span><span class="sxs-lookup"><span data-stu-id="89282-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="89282-106">Varmista, että käytät järjestelmän verkkonäkymää tai järjestelmäselainta, kun kirjaudut sisään käyttäjiisi kuluttaja-Google-tileillä.</span><span class="sxs-lookup"><span data-stu-id="89282-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="89282-107">Lisätietoja on kohdassa [Sovellukseen kirjautumisongelmat vain Chrome-selaimella.](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)</span><span class="sxs-lookup"><span data-stu-id="89282-107">For more information, see [Issues signing in to application(s) using Chrome browser only](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="89282-108">**En voi luoda uutta käyttäjää Azure AD -hakemistoon**</span><span class="sxs-lookup"><span data-stu-id="89282-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="89282-109">Varmista, että sinulla on oikeus luoda uusi peruskäyttäjä.</span><span class="sxs-lookup"><span data-stu-id="89282-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="89282-110">Vain yleinen järjestelmänvalvoja tai käyttäjän järjestelmänvalvojan Azure Active Directory (AD) voi luoda uuden peruskäyttäjän.</span><span class="sxs-lookup"><span data-stu-id="89282-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="89282-111">Jos et kuulu näihin rooleihin, pyydä järjestelmänvalvojaa lisäämään sinut näihin rooleihin tai luomaan uusi käyttäjätili.</span><span class="sxs-lookup"><span data-stu-id="89282-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="89282-112">Varmista, että käyttäjänimi on Toimialueessa, joka on vahvistettu Azure AD:ssä.</span><span class="sxs-lookup"><span data-stu-id="89282-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="89282-113">Jos Azure AD:ssä ei ole vahvistettuja mukautettuja toimialuenimiä, voit käyttää Azure AD:n alkuperäistä toimialuetta, jonka lopussa on \*.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="89282-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="89282-114">Varmista, että käyttäjänimi on toimialueella, jota ei ole liitetty Azure AD:iin paikallisesta AD:stä.</span><span class="sxs-lookup"><span data-stu-id="89282-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="89282-115">Käyttäjiä ei voi lisätä pilvipalveluun toimialuenimillä, jotka on liitetty paikallisesti.</span><span class="sxs-lookup"><span data-stu-id="89282-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="89282-116">Varmista, että toisella käyttäjällä tai yhteyshenkilöllä ei ole vielä käyttäjänimiä, jonka haluat määrittää uudelle käyttäjälle.</span><span class="sxs-lookup"><span data-stu-id="89282-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="89282-117">Käyttäjien nimien on oltava yksilöllisiä Azure AD:ssä.</span><span class="sxs-lookup"><span data-stu-id="89282-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="89282-118">Tutustu [Azure AD:n rooleihin ja järjestelmänvalvojiin](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD:ssä.</span><span class="sxs-lookup"><span data-stu-id="89282-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="89282-119">Katso Azure [AD:n](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) toimialuenimet.</span><span class="sxs-lookup"><span data-stu-id="89282-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="89282-120">Tarkista [valvontalokit,](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) jos haluat nähdä yksityiskohtaisempia tietoja äskettäin luodusta tai poistetusta käyttäjästä, kuten toiminnon suorittavasta henkilöstä ja milloin.</span><span class="sxs-lookup"><span data-stu-id="89282-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="89282-121">Lisätietoja uusien käyttäjien lisäämisestä on kohdassa Uuden käyttäjän luominen Azure AD:ssä [Azure-portaalin avulla.](/azure/active-directory/active-directory-users-create-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="89282-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="89282-122">[Azure AD:n järjestelmänvalvojan roolit:](/azure/active-directory/active-directory-assign-admin-roles)järjestelmänvalvojan roolin Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="89282-122">[Azure AD administrative roles](/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="89282-123">Voit luoda uuden [käyttäjän myös Azure AD PowerShellin avulla.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="89282-123">You can also [use Azure AD PowerShell to create a new user](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>
