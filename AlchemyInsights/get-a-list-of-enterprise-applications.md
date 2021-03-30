---
title: Enterprise-sovellusten luettelon hakeminen
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
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404529"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="ff095-102">Enterprise-sovellusten luettelon hakeminen</span><span class="sxs-lookup"><span data-stu-id="ff095-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="ff095-103">Saat  [PowerShell-komennolla](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)luettelon yrityssovelluksista (kaikki sovellukset tai näyttönimen, tunnuksen, tunnisteen TUNNUKSIA jne.) -suodatuksen.</span><span class="sxs-lookup"><span data-stu-id="ff095-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="ff095-104">Jos haluat nähdä luettelon palvelun pääobjekteista (kaikki objektit tai suodatetaan tunnuksen mukaan) PowerShell-komennolla, katso [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span><span class="sxs-lookup"><span data-stu-id="ff095-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="ff095-105">Jos haluat saada **luettelon SAML:n määritetyistä sovelluksista, seuraavista PowerShell-komentosarjoista** voi olla apua:</span><span class="sxs-lookup"><span data-stu-id="ff095-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="ff095-106">Jokaisessa sovelluksessa on OAuth-sovellus tai SAML-sovellus (sekä valikoima- että muut kuin valikoimasovellukset) kaksi objektia, jotka on luotu AAD:ssä, kun rekisteröinti tapahtuu.</span><span class="sxs-lookup"><span data-stu-id="ff095-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="ff095-107">Toista kutsutaan sovellusobjektiksi ja toinen palvelun pääobjektiksi.</span><span class="sxs-lookup"><span data-stu-id="ff095-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="ff095-108">Kun lisäät vedoksen Service Principal -objektin ominaisuuksiin PowerShellin avulla, jokaiseen sovellukseen liittyy tietty määrä tunnisteita:</span><span class="sxs-lookup"><span data-stu-id="ff095-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="ff095-109">OAuth-sovelluksissa olisi tunniste nimeltä "**WindowsAzureActiveDirectoryIntegratedApp**"</span><span class="sxs-lookup"><span data-stu-id="ff095-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="ff095-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="ff095-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="ff095-111">Muut kuin galleriat -SAML-sovelluksissa olisi tunniste nimeltä "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span><span class="sxs-lookup"><span data-stu-id="ff095-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="ff095-112">Näin ollen voit käyttää näitä tunnisteita ja selvittää, millainen sovellus se on.</span><span class="sxs-lookup"><span data-stu-id="ff095-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="ff095-113">Tunniste "**WindowsAzureActiveDirectoryIntegratedApp**" on yleinen kaikentyyppisille sovelluksille.</span><span class="sxs-lookup"><span data-stu-id="ff095-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="ff095-114">Seuraavan katkelman avulla voit luetella kaikki SAML-sovellukset (sekä valikoimat että muut kuin valikoimat):</span><span class="sxs-lookup"><span data-stu-id="ff095-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="ff095-115">Lisätietoja on kohdassa [SAML-yhteensopivien sovellusten tunnistaminen Azure AD:ssä.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)</span><span class="sxs-lookup"><span data-stu-id="ff095-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="ff095-116">**Vain verkkosovellusten etsiminen** ja luetteloiminen: Käytä alla olevaa komentoa, kun haluat hankkia kaikki Azure AD -sovellukset, joiden sovellustyyppi on "Verkkosovellus/ohjelmointirajapinta".</span><span class="sxs-lookup"><span data-stu-id="ff095-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="ff095-117">Get-AzureADApplication -Kaikki:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="ff095-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="ff095-118">**Etsi ja luetella alkuperäisiä sovelluksia** yksikseen: Suorita seuraava komento, niin saat kaikki alkuperäiset asiakassovellukset (työpöytä-/mobiililaitteet).</span><span class="sxs-lookup"><span data-stu-id="ff095-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="ff095-119">Get-AzureADApplication -Kaikki:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="ff095-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="ff095-120">**Vie kaikki rekisteröidyt Azure AD -sovelluksen tiedot** CSV-tiedostoon: Alla oleva komento vie kaikki Azure AD -sovellukset, joissa on tarvittavat tiedot csv-tiedostoon:</span><span class="sxs-lookup"><span data-stu-id="ff095-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="ff095-121">Get-AzureADApplication -Kaikki:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="ff095-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="ff095-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="ff095-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="ff095-123">**Käyttämättömien Azure-sovellusten luettelon vieminen** – valvontaraportti</span><span class="sxs-lookup"><span data-stu-id="ff095-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="ff095-124">Azure AD voi näyttää sovelluslokit vain 30 päivän ajan, jos sinulla on Azure AD Premium -käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="ff095-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="ff095-125">Voit säilyttää tiedot 30 päivän ajan kahdella eri vaihtoehdolla.</span><span class="sxs-lookup"><span data-stu-id="ff095-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="ff095-126">Voit noutaa tiedot [ohjelmallisesti ja](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) tallentaa ne tietokantaan Azure AD Reporting -ohjelmointirajapintojen avulla.</span><span class="sxs-lookup"><span data-stu-id="ff095-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="ff095-127">Voit myös integroida valvontalokit kolmannen osapuolen SIEM-järjestelmään.</span><span class="sxs-lookup"><span data-stu-id="ff095-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="ff095-128">Voit myös ladata sovellusluettelon kaikkiin sovelluksiin ja omistamuksiin Azure Active Directoryn alla,>sovellusten rekisteröinnit>ladata>kaikki sovellukset /omistavat sovellukset.</span><span class="sxs-lookup"><span data-stu-id="ff095-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="ff095-129">Jos haluat saada luettelon sovelluksista MS Graphin kautta, katso [Luettelosovellukset – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) ja sovellusresurssityyppi – Microsoft Graph [v1.0.](https://docs.microsoft.com/graph/api/resources/application)</span><span class="sxs-lookup"><span data-stu-id="ff095-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
