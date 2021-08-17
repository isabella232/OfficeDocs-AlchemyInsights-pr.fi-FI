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
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116725"
---
# <a name="get-a-list-of-enterprise-applications"></a>Enterprise-sovellusten luettelon hakeminen

1. Saat  Powershell-komennolla luettelon yrityssovelluksista (kaikki sovellukset tai näyttönimen, tunnuksen tai tunnisteiden TUNNUKSIEN mukaan suodatetut sovellukset) artikkelista [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)
2. Jos haluat nähdä luettelon palvelun pääobjekteista (kaikki objektit tai suodatetut tunnuksen mukaan) PowerShell-komennon avulla, katso [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)
3. Jos haluat saada **luettelon SAML-määritetyistä sovelluksista, seuraavista PowerShell-komentosarjoista** voi olla apua:

    Jokaisessa sovelluksessa on OAuth-sovellus tai SAML-sovellus (sekä valikoima- että ei-valikoimasovellukset) kaksi objektia luotuna AAD:ssä, kun niiden rekisteröinti tapahtuu. Toista kutsutaan Sovellusobjektiksi ja toinen palvelun pääobjektiksi. Kun lisäätvedoksen Service Principal -objektin ominaisuuksiin PowerShellin avulla, jokaisessa sovelluksessa on tietty määrä tunnisteita:

    - OAuth-sovelluksissa olisi tunniste nimeltä "**WindowsAzureActiveDirectoryIntegratedApp**"
    - Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Muut kuin valikoimat SAML-sovelluksissa olisi tunniste nimeltä "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Näin ollen voit käyttää näitä tunnisteita ja selvittää, millainen sovellus se on. Tunniste "**WindowsAzureActiveDirectoryIntegratedApp**" on yleinen kaikissa sovellustyypeissä. Seuraavan katkelman avulla voit luetella kaikki SAML-sovellukset (sekä valikoima että muut kuin valikoimat):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Lisätietoja on kohdassa [SAML-yhteensopivien sovellusten tunnistaminen Azure AD:ssä.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **Vain verkkosovellusten etsiminen ja** luetteloiminen: Käytä alla olevaa komentoa, kun haluat käyttää kaikkia Azure AD -sovelluksia, joiden sovellustyyppi on "Verkkosovellus/ohjelmointirajapinta".

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } -| FT
5. **Etsi ja luetteloi vain alkuperäiset sovellukset:** Suorita seuraava komento, niin saat kaikki alkuperäiset asiakassovellukset (työpöytä-/mobiililaitesovellukset).

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } -| FT
6. **Vie kaikki rekisteröidyt Azure AD -sovelluksen tiedot** CSV-tiedostoon: Alla oleva komento vie kaikki Azure AD -sovellukset, joissa on tarvittavat tiedot csv-tiedostoon:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Luettelo käyttämättömistä Azure-sovelluksista** on vietävä – valvontaraportti

    Azure AD voi näyttää sovelluslokit vain 30 päivän ajan, jos sinulla on Azure AD Premium käyttöoikeus.
    Voit säilyttää tietoja yli 30 päivän ajan kahdella eri vaihtoehdolla. Voit noutaa tiedot [ohjelmallisesti ja](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) tallentaa ne tietokantaan Azure AD Reporting -ohjelmointirajapintojen avulla. Voit myös integroida valvontalokit kolmannen osapuolen SIEM-järjestelmään.

    Voit myös ladata sovellusluettelon kaikista sovelluksista ja omistamistasi sovelluksista Azure Active Directoryn>app registrations>Download>All applications/Owned applications (Kaikki sovellukset/omistamat sovellukset).

    Jos haluat saada luettelon sovelluksista MS Graph:n kautta, katso [Luettelosovellukset – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) ja sovellusresurssityyppi – Microsoft Graph versio [1.0.](https://docs.microsoft.com/graph/api/resources/application)
