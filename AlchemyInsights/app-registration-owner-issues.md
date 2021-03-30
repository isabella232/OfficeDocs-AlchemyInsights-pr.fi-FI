---
title: Sovelluksen rekisteröintiomistajan ongelmat
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
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404456"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="5fd9b-102">Sovelluksen rekisteröintiomistajan ongelmat</span><span class="sxs-lookup"><span data-stu-id="5fd9b-102">App Registration Owner issues</span></span>

<span data-ttu-id="5fd9b-103">Seuraavassa on menetelmät, joilla voit lisätä päätoimitsijat sovellusrekisteröinnit omistajiksi:</span><span class="sxs-lookup"><span data-stu-id="5fd9b-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="5fd9b-104">Azure AD PowerShell -moduulin käyttäminen –</span><span class="sxs-lookup"><span data-stu-id="5fd9b-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="5fd9b-105">Viite: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="5fd9b-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="5fd9b-106">Azure CLI :n käyttäminen - `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="5fd9b-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="5fd9b-107">Viite: [az ad -sovelluksen omistaja](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="5fd9b-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="5fd9b-108">MS Graphin käyttäminen -</span><span class="sxs-lookup"><span data-stu-id="5fd9b-108">Using MS Graph -</span></span>

    <span data-ttu-id="5fd9b-109">Viite: [Omistajan lisääminen – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="5fd9b-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="5fd9b-110">Azure AD -portaalin käyttäminen – Siirry [portal.azure.com](https://portal.azure.com/) > Azure Active Directoryyn > sovelluksen rekisteröintisovelluksen > Valitse > Omistajat > Lisää omistajia</span><span class="sxs-lookup"><span data-stu-id="5fd9b-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="5fd9b-111">**Etkö voi tarkastella sovellusta sovelluksen rekisteröintien lavatta, vaikka olet sovelluksen omistaja?**</span><span class="sxs-lookup"><span data-stu-id="5fd9b-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="5fd9b-112">Sovelluksen omistaja ei ole järjestelmänvalvojarooli.</span><span class="sxs-lookup"><span data-stu-id="5fd9b-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="5fd9b-113">Jos Rajoita azure [AD -hallintaportaalin](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) käyttöä -asetus on käytössä, vain järjestelmänvalvoja voi tarkastella sovelluksia sovelluksen rekisteröintiportaalissa.</span><span class="sxs-lookup"><span data-stu-id="5fd9b-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="5fd9b-114">Jotta omistaja voi tarkastella sovelluksia, joko poistaa tämän asetuksen käytöstä (Aseta asetukseksi EI) tai määrittää järjestelmänvalvojan roolin omistajalle vain tietyssä sovelluksessa.</span><span class="sxs-lookup"><span data-stu-id="5fd9b-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="5fd9b-115">Tätä varten tarvitset kuitenkin Azure AD Premium P2 -käyttöoikeuden ja otat [Privileged Identity Managementin käyttöön.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="5fd9b-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
