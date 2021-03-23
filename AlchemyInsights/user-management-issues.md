---
title: Käyttäjien hallintaongelmat
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035532"
---
# <a name="user-management-issues"></a><span data-ttu-id="8df63-102">Käyttäjien hallintaongelmat</span><span class="sxs-lookup"><span data-stu-id="8df63-102">User management issues</span></span>

<span data-ttu-id="8df63-103">**Mitä tapahtuu nykyisille määritetyille käyttäjille sovellukselle, jos poistan käyttäjämäärityksen pakollisen ominaisuuden käytöstä (asetan tämän ominaisuuden arvoksi Ei)?**</span><span class="sxs-lookup"><span data-stu-id="8df63-103">**What happens to current assigned users to the application if I disable the property ‘User assignment required’ (set this property to No)?**</span></span>

<span data-ttu-id="8df63-104">Käyttäjän **pakollisen tehtävän poistaminen käytöstä** EI vaikuta tällä hetkellä määritettyihin käyttäjiin.</span><span class="sxs-lookup"><span data-stu-id="8df63-104">Disabling **User assignment required** does NOT affect the currently assigned users.</span></span> <span data-ttu-id="8df63-105">Jos poistat tämän ominaisuuden käytöstä, kaikki käyttäjät voivat käyttää sovellusta.</span><span class="sxs-lookup"><span data-stu-id="8df63-105">Disabling this property will only allow all users to access the application.</span></span> <span data-ttu-id="8df63-106">Kaikki luettelossa mainitut käyttäjät ja ryhmille sovelluksessa määritetyt käyttäjät ovat edelleen kelvollisia.</span><span class="sxs-lookup"><span data-stu-id="8df63-106">All the listed users and those users assigned to groups in the application will still be valid.</span></span>

- <span data-ttu-id="8df63-107">Jos haluat rajoittaa sovelluksen tietyille käyttäjille, katso kohta - Azure AD -sovelluksen rajoittaminen käyttäjäjoukolle [– Microsoftin käyttäjätietoympäristön | Microsoft Docs.](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.)</span><span class="sxs-lookup"><span data-stu-id="8df63-107">To restrict your app to specific set of users, see - [Restrict Azure AD app to a set of users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span></span>
- <span data-ttu-id="8df63-108">Jos haluat määrittää käyttäjiä ja ryhmiä, azure Active Directoryn (Azure AD) yrityssovelluksiin joko Azure-portaalista tai PowerShellin avulla, katso lisätietoja artikkelista Sovelluksen käyttäjämäärityksen hallinta [Azure Active Directoryssa.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)</span><span class="sxs-lookup"><span data-stu-id="8df63-108">To assign users and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell, see [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span></span>
- <span data-ttu-id="8df63-109">Jos haluat delegoida sovellusten luonti- ja hallintaoikeuksia, katso kohta [Edustajasovelluksen hallinnan järjestelmänvalvojan oikeudet – Azure AD | Microsoft Docs.](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles)</span><span class="sxs-lookup"><span data-stu-id="8df63-109">To delegate Application creation and management permissions, see [Delegate application management administrator permissions - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span></span>
- <span data-ttu-id="8df63-110">**Piilota tietyt yrityssovellukset käyttäjiltä** – Voit piilottaa kaikki Microsoft 365 -sovellukset **MyApps-paneelista** seuraavasti.</span><span class="sxs-lookup"><span data-stu-id="8df63-110">**Hide specific enterprise apps from users** - Use the following steps to hide all Microsoft 365 apps from the **MyApps** panel.</span></span> <span data-ttu-id="8df63-111">Sovellukset näkyvät edelleen Office 365 -portaalissa.</span><span class="sxs-lookup"><span data-stu-id="8df63-111">The apps will still be visible in the Office 365 portal.</span></span>

 1. <span data-ttu-id="8df63-112">Kirjaudu Azure-portaaliin hakemiston yleisenä järjestelmänvalvojana.</span><span class="sxs-lookup"><span data-stu-id="8df63-112">Sign-in to the Azure portal as a global administrator for your directory.</span></span> 
 2. <span data-ttu-id="8df63-113">Valitse **Azure Active Directory.**</span><span class="sxs-lookup"><span data-stu-id="8df63-113">Select **Azure Active Directory**.</span></span> 
 3. <span data-ttu-id="8df63-114">Valitse **Käyttäjät**.</span><span class="sxs-lookup"><span data-stu-id="8df63-114">Select **Users**.</span></span> 
 4. <span data-ttu-id="8df63-115">Valitse **Käyttäjäasetukset.**</span><span class="sxs-lookup"><span data-stu-id="8df63-115">Select **User settings**.</span></span> 
 5. <span data-ttu-id="8df63-116">Valitse **Yrityssovellukset-kohdassa** **Hallitse käyttäjien käynnistys- ja tarkastelemissovelluksia.**</span><span class="sxs-lookup"><span data-stu-id="8df63-116">Under **Enterprise applications**, click **Manage how end users launch and view their applications**.</span></span> 
 6. <span data-ttu-id="8df63-117">Käyttäjät **näkevät Office 365 -sovellukset vain Office 365 -portaalissa, ja valitse** **Kyllä.**</span><span class="sxs-lookup"><span data-stu-id="8df63-117">For **Users can only see Office 365 apps in the Office 365 portal**, click **Yes**.</span></span> 
 7. <span data-ttu-id="8df63-118">Valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="8df63-118">Click **Save**.</span></span> 
 8. <span data-ttu-id="8df63-119">Lisätietoja on kohdassa [Yrityssovelluksen piilottaminen käyttäjäkokemukselta Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span><span class="sxs-lookup"><span data-stu-id="8df63-119">For more details, see [Hide an Enterprise application from user's experience in Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span></span>

- <span data-ttu-id="8df63-120">Jos tarjoat Ohjelmisto palveluna (SaaS) -sovellusta useille organisaatioille, voit määrittää sovelluksesi hyväksymään minkä tahansa Azure Active Directory (Azure AD) -vuokraajan kirjautumiset.</span><span class="sxs-lookup"><span data-stu-id="8df63-120">If you offer a Software as a Service (SaaS) app to many organizations, you can configure your app to accept sign-ins from any Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="8df63-121">Tätä kokoonpanoa kutsutaan "sovelluksen moni vuokraajaksi".</span><span class="sxs-lookup"><span data-stu-id="8df63-121">This configuration is called "making your application multi-tenant".</span></span> <span data-ttu-id="8df63-122">Minkä tahansa Azure AD -vuokraajan käyttäjät voivat kirjautua sovellukseesi, kun he ovat suostuneet käyttämään tiliään sovelluksessasi.</span><span class="sxs-lookup"><span data-stu-id="8df63-122">Users in any Azure AD tenant will be able to sign-in to your app after consenting to use their account with your app.</span></span> <span data-ttu-id="8df63-123">Lisätietoja on kohdassa Azure [AD -käyttäjiin kirjautumisen sovellusten luominen – Microsoftin | Microsoft Docs.](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant)</span><span class="sxs-lookup"><span data-stu-id="8df63-123">For more information, see [Build apps that sign in Azure AD users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span></span>

- <span data-ttu-id="8df63-124">**Miten loppukäyttäjä voi käyttää sovellusta, kun hänet on määritetty sovellukseen?**</span><span class="sxs-lookup"><span data-stu-id="8df63-124">**How can an end user access the application once he/she is assigned to the application?**</span></span>

<span data-ttu-id="8df63-125">Jokaisella Enterprise-sovelluksen sovelluksella on linkki loppukäyttäjille.</span><span class="sxs-lookup"><span data-stu-id="8df63-125">Each app in Enterprise application blade has a link for end users to access.</span></span> <span data-ttu-id="8df63-126">Käyttäjät voivat käyttää sovellusta myös **MyApps-portaalin** kautta helposti.</span><span class="sxs-lookup"><span data-stu-id="8df63-126">Users can also access the app through **Myapps** portal in an easy way.</span></span>

- <span data-ttu-id="8df63-127">**Haluatko tietää, mitä sovelluksia ja sovelluksia käyttäjät käyttävät?**</span><span class="sxs-lookup"><span data-stu-id="8df63-127">**Want to know which applications and type of applications are being used by users?**</span></span>

<span data-ttu-id="8df63-128">Voit ladata kirjautumisraportit viimeisten 30 päivän ajan **portal.azure.com > Azure Active Directorysta> Signins> lataa raportteja.**</span><span class="sxs-lookup"><span data-stu-id="8df63-128">You can download sign-in reports for the last 30 days from **portal.azure.com > Azure Active directory> Signins> download reports**.</span></span>

- <span data-ttu-id="8df63-129">Lue, miten [voit myöntää vuokraajan laajuiselle järjestelmänvalvojalle](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) sovelluksen suostumuksen ja [määrittää, miten loppukäyttäjät hyväksyvät sovellukset.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)</span><span class="sxs-lookup"><span data-stu-id="8df63-129">Learn how to [Grant tenant wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) and [Configure how end users consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).</span></span>

- <span data-ttu-id="8df63-130">[Ymmärrät, miten suostumus toimii,](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) [ja hallitse sovellusten suostumusta.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)</span><span class="sxs-lookup"><span data-stu-id="8df63-130">Understand [how consent works](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) and [Manage consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).</span></span>


