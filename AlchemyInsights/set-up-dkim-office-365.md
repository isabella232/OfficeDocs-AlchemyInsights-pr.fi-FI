---
title: DKIM:n määrittäminen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645669"
---
# <a name="setup-dkim"></a><span data-ttu-id="cf89d-102">DKIM:n määrittäminen</span><span class="sxs-lookup"><span data-stu-id="cf89d-102">Setup DKIM</span></span>

<span data-ttu-id="cf89d-103">Täydelliset ohjeet DKIM:n määrittämiseen microsoft 365:n mukautetuille toimialueille ovat [täällä](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="cf89d-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="cf89d-104">**Jokaiselle** mukautetulle toimialueelle on luotava **kaksi** DKIM CNAME -tietuetta toimialueen DNS-isännöintipalveluun (yleensä toimialueen rekisteröintipalveluun).</span><span class="sxs-lookup"><span data-stu-id="cf89d-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="cf89d-105">Esimerkiksi contoso.com ja fourthcoffee.com edellyttää neljää DKIM CNAME -tietuetta: kaksi contoso.com ja kaksi fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="cf89d-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="cf89d-106">**Kunkin** mukautetun toimialueen DKIM CNAME -tietueet käyttävät seuraavia muotoja:</span><span class="sxs-lookup"><span data-stu-id="cf89d-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="cf89d-107">**Isännän nimi**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="cf89d-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="cf89d-108">**Osoite- tai arvopisteet:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="cf89d-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="cf89d-109">**Kävi koulua TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="cf89d-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="cf89d-110">**Isännän nimi**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="cf89d-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="cf89d-111">**Osoite- tai arvopisteet:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="cf89d-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="cf89d-112">**Kävi koulua TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="cf89d-112">**TTL**: 3600</span></span>

   <span data-ttu-id="cf89d-113">\<DomainGUID\> on mukautetun toimialueen `.mail.protection.outlook.com` mukautetun MX-tietueen (esimerkiksi `contoso-com` toimialueen contoso.com) mukautetun MX-tietueen vasemmalla puolella oleva teksti.</span><span class="sxs-lookup"><span data-stu-id="cf89d-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="cf89d-114">\<InitialDomain\> on toimialue, jota käytit rekisteröityessäsi Microsoft 365:een (esimerkiksi contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="cf89d-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="cf89d-115">Kun olet luonut Mukautettujen toimialueiden CNAME-tietueet, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="cf89d-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="cf89d-116">A.</span><span class="sxs-lookup"><span data-stu-id="cf89d-116">a.</span></span> <span data-ttu-id="cf89d-117">[kirjaudu Microsoft 365:een](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) työpaikan tai oppilaitoksen tilillä.</span><span class="sxs-lookup"><span data-stu-id="cf89d-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="cf89d-118">B.</span><span class="sxs-lookup"><span data-stu-id="cf89d-118">b.</span></span> <span data-ttu-id="cf89d-119">Valitse vasemmasta yläkulmasta sovellusten käynnistyskuvake ja valitse **Järjestelmänvalvoja**.</span><span class="sxs-lookup"><span data-stu-id="cf89d-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="cf89d-120">C.</span><span class="sxs-lookup"><span data-stu-id="cf89d-120">c.</span></span> <span data-ttu-id="cf89d-121">Laajenna vasemmassa alakulmassa **Järjestelmänvalvoja** ja valitse **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="cf89d-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="cf89d-122">D.</span><span class="sxs-lookup"><span data-stu-id="cf89d-122">d.</span></span> <span data-ttu-id="cf89d-123">Siirry **Kohtaan Suojaus** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="cf89d-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="cf89d-124">E.</span><span class="sxs-lookup"><span data-stu-id="cf89d-124">e.</span></span> <span data-ttu-id="cf89d-125">Valitse toimialue ja valitse sitten **Ota käyttöön** tämän **toimialueen Sign-viesteille DKIM-allekirjoituksilla**.</span><span class="sxs-lookup"><span data-stu-id="cf89d-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="cf89d-126">Toista tämä vaihe jokaisen mukautetun toimialueen kohdalla.</span><span class="sxs-lookup"><span data-stu-id="cf89d-126">Repeat this step for each custom domain.</span></span>
