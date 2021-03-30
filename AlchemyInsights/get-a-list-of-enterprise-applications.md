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
# <a name="get-a-list-of-enterprise-applications"></a>Enterprise-sovellusten luettelon hakeminen

1. Saat  [PowerShell-komennolla](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)luettelon yrityssovelluksista (kaikki sovellukset tai näyttönimen, tunnuksen, tunnisteen TUNNUKSIA jne.) -suodatuksen.
2. Jos haluat nähdä luettelon palvelun pääobjekteista (kaikki objektit tai suodatetaan tunnuksen mukaan) PowerShell-komennolla, katso [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).
3. Jos haluat saada **luettelon SAML:n määritetyistä sovelluksista, seuraavista PowerShell-komentosarjoista** voi olla apua:

    Jokaisessa sovelluksessa on OAuth-sovellus tai SAML-sovellus (sekä valikoima- että muut kuin valikoimasovellukset) kaksi objektia, jotka on luotu AAD:ssä, kun rekisteröinti tapahtuu. Toista kutsutaan sovellusobjektiksi ja toinen palvelun pääobjektiksi. Kun lisäät vedoksen Service Principal -objektin ominaisuuksiin PowerShellin avulla, jokaiseen sovellukseen liittyy tietty määrä tunnisteita:

    - OAuth-sovelluksissa olisi tunniste nimeltä "**WindowsAzureActiveDirectoryIntegratedApp**"
    - Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Muut kuin galleriat -SAML-sovelluksissa olisi tunniste nimeltä "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Näin ollen voit käyttää näitä tunnisteita ja selvittää, millainen sovellus se on. Tunniste "**WindowsAzureActiveDirectoryIntegratedApp**" on yleinen kaikentyyppisille sovelluksille. Seuraavan katkelman avulla voit luetella kaikki SAML-sovellukset (sekä valikoimat että muut kuin valikoimat):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Lisätietoja on kohdassa [SAML-yhteensopivien sovellusten tunnistaminen Azure AD:ssä.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **Vain verkkosovellusten etsiminen** ja luetteloiminen: Käytä alla olevaa komentoa, kun haluat hankkia kaikki Azure AD -sovellukset, joiden sovellustyyppi on "Verkkosovellus/ohjelmointirajapinta".

    Get-AzureADApplication -Kaikki:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Etsi ja luetella alkuperäisiä sovelluksia** yksikseen: Suorita seuraava komento, niin saat kaikki alkuperäiset asiakassovellukset (työpöytä-/mobiililaitteet).

    Get-AzureADApplication -Kaikki:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Vie kaikki rekisteröidyt Azure AD -sovelluksen tiedot** CSV-tiedostoon: Alla oleva komento vie kaikki Azure AD -sovellukset, joissa on tarvittavat tiedot csv-tiedostoon:

    - Get-AzureADApplication -Kaikki:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Käyttämättömien Azure-sovellusten luettelon vieminen** – valvontaraportti

    Azure AD voi näyttää sovelluslokit vain 30 päivän ajan, jos sinulla on Azure AD Premium -käyttöoikeus.
    Voit säilyttää tiedot 30 päivän ajan kahdella eri vaihtoehdolla. Voit noutaa tiedot [ohjelmallisesti ja](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) tallentaa ne tietokantaan Azure AD Reporting -ohjelmointirajapintojen avulla. Voit myös integroida valvontalokit kolmannen osapuolen SIEM-järjestelmään.

    Voit myös ladata sovellusluettelon kaikkiin sovelluksiin ja omistamuksiin Azure Active Directoryn alla,>sovellusten rekisteröinnit>ladata>kaikki sovellukset /omistavat sovellukset.

    Jos haluat saada luettelon sovelluksista MS Graphin kautta, katso [Luettelosovellukset – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) ja sovellusresurssityyppi – Microsoft Graph [v1.0.](https://docs.microsoft.com/graph/api/resources/application)
