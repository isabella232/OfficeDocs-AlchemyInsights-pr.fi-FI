---
title: Ohjelmointirajapintojen kanssa kehittyvien sovellusten ongelmat
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974618"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="7bf12-102">Sovellusten ohjelmointirajapintojen kehittämiseen liittyvät ongelmat</span><span class="sxs-lookup"><span data-stu-id="7bf12-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="7bf12-103">Jos haluat aloittaa Azure Active Directory Graph -ohjelmointirajapinnan käytön, tutustu [Azure AD Graph API:n pika-aloitusoppaaseen](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) tai tarkastele vuorovaikutteisia [Azure AD Graph -ohjelmointirajapinnan viitedokumentaatioita.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)</span><span class="sxs-lookup"><span data-stu-id="7bf12-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="7bf12-104">**Azure Active Directory -todennuskirjaston (ADAL) ja Azure AD Graph API:n (AAD Graph) tuen päättyminen**</span><span class="sxs-lookup"><span data-stu-id="7bf12-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="7bf12-105">**30. kesäkuuta 2020** alkaen uusia ominaisuuksia ei enää lisätä ADAL:een ja Azure AD Graphiin.</span><span class="sxs-lookup"><span data-stu-id="7bf12-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="7bf12-106">Teknisen tuen ja suojauspäivitysten tarjoaminen jatkuu, mutta ominaisuuspäivityksiä ei enää tarjota.</span><span class="sxs-lookup"><span data-stu-id="7bf12-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="7bf12-107">**30. kesäkuuta 2022** alkaen microsoft lopettaa ADAL: n ja Azure AD Graphin tuen, eikä se enää tarjoa teknistä tukea tai suojauspäivityksiä.</span><span class="sxs-lookup"><span data-stu-id="7bf12-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="7bf12-108">Sovellukset, jotka käyttävät ADAL:tä nykyisissä käyttöjärjestelmäversioissa, toimivat edelleen tämän ajan kuluttua, mutta eivät saa teknistä tukea tai suojauspäivityksiä.</span><span class="sxs-lookup"><span data-stu-id="7bf12-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="7bf12-109">Azure AD Graphia tämän jälkeen käyttävät sovellukset eivät ehkä enää saa vastauksia Azure AD Graph -päätepisteltä.</span><span class="sxs-lookup"><span data-stu-id="7bf12-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="7bf12-110">**ADAL-siirto**</span><span class="sxs-lookup"><span data-stu-id="7bf12-110">**ADAL Migration**</span></span>

<span data-ttu-id="7bf12-111">Suosittelemme päivittämään [Microsoftin todentamiskirjastoon (MSAL),](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)jossa on uusimmat ominaisuudet ja suojauspäivitykset.</span><span class="sxs-lookup"><span data-stu-id="7bf12-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="7bf12-112">Jos käytät Microsoft-sovelluksia, tiedät, että Microsoft on parhaillaan muuttamassa sovelluksiaan MSAL-sovelluksiin tuen päättymiseen mennessä, jotta ne hyötyvät MSAL:n käynnissä olevista suojaus- ja ominaisuusparannuksista.</span><span class="sxs-lookup"><span data-stu-id="7bf12-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="7bf12-113">[Lue ADAL:n usein kysytyt kysymykset.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="7bf12-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="7bf12-114">[Lue lisää siitä, miten voit siirtää sovelluksia käyttöympäristökohtaisesti.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="7bf12-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="7bf12-115">Jos tarvitset apua sen ymmärtämiseen, mitkä sovellukset käyttävät ADAL:tä, suosittelemme tarkistamaan kaikki sovellusten lähdekoodit ja tarvittaessa ottaa yhteyttä internet-palveluntarjoajiin tai sovellustarjoajiin.</span><span class="sxs-lookup"><span data-stu-id="7bf12-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="7bf12-116">Microsoft-tuki voi myös tarjota sinulle luettelon kaikista vuokraajan ei-Microsoft ADAL -sovelluksista.</span><span class="sxs-lookup"><span data-stu-id="7bf12-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="7bf12-117">**AAD Graph -siirto**</span><span class="sxs-lookup"><span data-stu-id="7bf12-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="7bf12-118">Jos sovellus käyttää Azure AD Graphia, noudata ohjeita azure AD Graph -sovellusten [siirtämiseksi Microsoft Graphiin.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="7bf12-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="7bf12-119">[Siirron tarkistusluettelomme tarjoaa aloituspisteen.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)</span><span class="sxs-lookup"><span data-stu-id="7bf12-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="7bf12-120">Azure-sovelluksen rekisteröintiportaali näyttää, mitkä sovellukset käyttävät AAD Graphia.</span><span class="sxs-lookup"><span data-stu-id="7bf12-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="7bf12-121">Suosittelemme, että tarkistat kaikki sovellusten lähdekoodit, ja ota tarvittaessa yhteyttä internet-palveluntarjoajiin tai sovelluspalveluntarjoajiin.</span><span class="sxs-lookup"><span data-stu-id="7bf12-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="7bf12-122">Microsoft-tuki voi myös tarjota sinulle luettelon vuokraajan kaikista AAD Graph -käytöstä.</span><span class="sxs-lookup"><span data-stu-id="7bf12-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="7bf12-123">Jotta sovellus voi käyttää Microsoft Graphin tietoja, käyttäjän tai järjestelmänvalvojan on myönnettävä se oikeat käyttöoikeudet suostumusprosessin kautta.</span><span class="sxs-lookup"><span data-stu-id="7bf12-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="7bf12-124">[Microsoft Graph -käyttöoikeusviittauksessa](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) luetellaan kuhunkin Microsoft Graph -ohjelmointirajapintojen pääjoukkoon liittyvät käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="7bf12-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="7bf12-125">Artikkelissa on myös ohjeita käyttöoikeuksien käyttöön.</span><span class="sxs-lookup"><span data-stu-id="7bf12-125">It also provides guidance about how to use the permissions.</span></span>
