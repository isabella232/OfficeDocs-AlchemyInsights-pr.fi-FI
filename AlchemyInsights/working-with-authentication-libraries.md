---
title: Todennuskirjastojen käyttäminen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035285"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="75d71-102">Todennuskirjastojen käyttäminen</span><span class="sxs-lookup"><span data-stu-id="75d71-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="75d71-103">Voit ratkaista Microsoftin todennuskirjaston (MSAL) ongelman noudattamalla seuraavia suositeltuja ohjeita:</span><span class="sxs-lookup"><span data-stu-id="75d71-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="75d71-104">**MSAL:n käyttäminen:** [Microsoftin käyttäjätietojen alustojen todennuskirjastot](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – Tässä artikkelissa kerrotaan Microsoftin todennuskirjaston tuesta useille sovellustyypeille.</span><span class="sxs-lookup"><span data-stu-id="75d71-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="75d71-105">Se sisältää linkkejä kirjaston lähdekoodiin; mistä saat paketin sovelluksen projektia varten ja tukeeko kirjasto käyttäjän kirjautumista (todennusta), suojattujen verkkorajapintojen (valtuutuksen) käyttö vai molemmat.</span><span class="sxs-lookup"><span data-stu-id="75d71-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="75d71-106">**Todennuksen** vianmääritys: MSAL tukee useita todennusvirtoja käytettäväksi eri sovellusskenaarioissa.</span><span class="sxs-lookup"><span data-stu-id="75d71-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="75d71-107">Sen mukaan, miten asiakassovellus on luotu, MSAL voi käyttää vähintään yhtä Microsoftin käyttäjätietoympäristön tukemista todennusvirroista.</span><span class="sxs-lookup"><span data-stu-id="75d71-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="75d71-108">Nämä työnkulut voivat tuottaa monenlaisia tunnuksia ja valtuutuskoodeja, ja niiden toimiminen edellyttää erilaisia tunnuksia.</span><span class="sxs-lookup"><span data-stu-id="75d71-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="75d71-109">**Access Tokens:** [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span><span class="sxs-lookup"><span data-stu-id="75d71-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="75d71-110">Kaikki tämän artikkelin ohjeet, paitsi jos ne on mainittu, koskevat vain rekisteröityjen ohjelmointirajapintojen tunnuksia.</span><span class="sxs-lookup"><span data-stu-id="75d71-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="75d71-111">Se ei koske Microsoftin omistamien ohjelmointirajapintojen tunnuksia eikä tunnuksia voida käyttää sen tarkistamiseen, miten Microsoftin tunnistetietoympäristö myöntää tunnuksia luomaasi ohjelmointirajapintaan.</span><span class="sxs-lookup"><span data-stu-id="75d71-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="75d71-112">**Azure Active Directory -todennuskirjaston (ADAL) tuen päättyminen**</span><span class="sxs-lookup"><span data-stu-id="75d71-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="75d71-113">**30. kesäkuuta 2020** alkaen uusia ominaisuuksia ei enää lisätä ADAL:een ja Azure AD Graphiin.</span><span class="sxs-lookup"><span data-stu-id="75d71-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="75d71-114">Tarjoamme jatkossakin teknistä tukea ja suojauspäivityksiä, mutta emme enää tarjoa ominaisuuspäivityksiä.</span><span class="sxs-lookup"><span data-stu-id="75d71-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="75d71-115">**30. kesäkuuta 2022** alkaen microsoft lopettaa ADAL: n ja Azure AD Graphin tuen, eikä se enää tarjoa teknistä tukea tai suojauspäivityksiä.</span><span class="sxs-lookup"><span data-stu-id="75d71-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="75d71-116">Sovellukset, jotka käyttävät ADAL:tä nykyisissä käyttöjärjestelmäversioissa, toimivat edelleen tämän ajan kuluttua, mutta eivät saa *teknistä tukea tai suojauspäivityksiä.*</span><span class="sxs-lookup"><span data-stu-id="75d71-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="75d71-117">Azure AD Graphia tämän jälkeen käyttävät sovellukset eivät ehkä enää saa vastauksia Azure AD Graph -päätepisteltä.</span><span class="sxs-lookup"><span data-stu-id="75d71-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="75d71-118">**ADAL-siirto**</span><span class="sxs-lookup"><span data-stu-id="75d71-118">**ADAL Migration**</span></span>

- <span data-ttu-id="75d71-119">Suosittelemme päivittämään MSAL-versioon, jossa on uusimmat ominaisuudet ja suojauspäivitykset.</span><span class="sxs-lookup"><span data-stu-id="75d71-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="75d71-120">Jos käytät Microsoft-sovelluksia, tiedät, että Microsoft on parhaillaan muuttamassa sovelluksiaan MSAL-sovelluksiin tuen päättymiseen mennessä, jotta ne hyötyvät MSAL:n käynnissä olevista suojaus- ja ominaisuusparannuksista.</span><span class="sxs-lookup"><span data-stu-id="75d71-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="75d71-121">[Lue ADAL:n usein kysytyt kysymykset.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="75d71-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="75d71-122">[Lue lisää siitä, miten voit siirtää sovelluksia käyttöympäristökohtaisesti.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)</span><span class="sxs-lookup"><span data-stu-id="75d71-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="75d71-123">Jos sinulla on lisäkysymyksiä sovelluksen käyttöympäristön oppaan lukemisen jälkeen, voit julkaista sen [Microsoftin kysymysten ja](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) kysymysten&A -tunnisteella [azure-ad-adal-deprecation] tai avata ongelman kirjaston GitHub-säilössä.</span><span class="sxs-lookup"><span data-stu-id="75d71-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="75d71-124">[MSAL-yleiskatsausartikkelin](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) Kielet  ja kehykset -osassa on linkkejä kunkin kirjaston repo-kohteeseen.</span><span class="sxs-lookup"><span data-stu-id="75d71-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="75d71-125">**Jos tarvitset apua ADAL-sovellusten** käytössä, suosittelemme tarkistamaan kaikki sovellusten lähdekoodit.</span><span class="sxs-lookup"><span data-stu-id="75d71-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="75d71-126">Ota tarvittaessa yhteyttä itsenäisten ohjelmistotoimittajien (ISV) tai sovellustoimittajien käyttöön.</span><span class="sxs-lookup"><span data-stu-id="75d71-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="75d71-127">Microsoftin tukipalvelu voi myös tarjota sinulle luettelon kaikista vuokraajan ei-Microsoft ADAL -sovelluksista.</span><span class="sxs-lookup"><span data-stu-id="75d71-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







