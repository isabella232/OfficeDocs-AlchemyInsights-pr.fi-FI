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
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509381"
---
# <a name="setup-dkim"></a><span data-ttu-id="27834-102">DKIM:n määrittäminen</span><span class="sxs-lookup"><span data-stu-id="27834-102">Setup DKIM</span></span>

<span data-ttu-id="27834-103">Täydelliset ohjeet DKIM:n määrittämiseen microsoft 365:n mukautetuille toimialueille ovat [täällä](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="27834-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="27834-104">**Jokaiselle** mukautetulle toimialueelle on luotava **kaksi** DKIM CNAME -tietuetta toimialueen DNS-isännöintipalvelussa (yleensä toimialueen rekisteröintipalvelu).</span><span class="sxs-lookup"><span data-stu-id="27834-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="27834-105">Esimerkiksi contoso.com ja fourthcoffee.com vaativat neljä DKIM CNAME -tietuetta: kaksi contoso.com ja kaksi fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="27834-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="27834-106">**Kunkin** mukautetun toimialueen DKIM CNAME -tietueissa käytetään seuraavia muotoja:</span><span class="sxs-lookup"><span data-stu-id="27834-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="27834-107">**Isännän nimi**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="27834-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="27834-108">**Osoite- tai arvopisteet:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="27834-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="27834-109">**TTL**: 3600 (alv.)</span><span class="sxs-lookup"><span data-stu-id="27834-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="27834-110">**Isännän nimi**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="27834-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="27834-111">**Osoite- tai arvopisteet:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="27834-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="27834-112">**TTL**: 3600 (alv.)</span><span class="sxs-lookup"><span data-stu-id="27834-112">**TTL**: 3600</span></span>

   <span data-ttu-id="27834-113">\<DomainGUID\>on mukautetun toimialueen mukautetun MX-tietueen vasemmalla puolella oleva teksti `.mail.protection.outlook.com` (esimerkiksi `contoso-com` toimialueen contoso.com).</span><span class="sxs-lookup"><span data-stu-id="27834-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="27834-114">\<InitialDomain\>on toimialue, jota käytit rekisteröityessäsi Microsoft 365:ään (esimerkiksi contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="27834-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="27834-115">Kun olet luonut CNAME-tietueet mukautetuille toimialueillesi, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="27834-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="27834-116">a.</span><span class="sxs-lookup"><span data-stu-id="27834-116">a.</span></span> <span data-ttu-id="27834-117">[kirjaudu Microsoft 365:lle](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) työpaikan tai oppilaitoksen tilillä.</span><span class="sxs-lookup"><span data-stu-id="27834-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="27834-118">b.</span><span class="sxs-lookup"><span data-stu-id="27834-118">b.</span></span> <span data-ttu-id="27834-119">Valitse vasemmasta yläkulmasta sovellusten käynnistyskuvake ja valitse **Järjestelmänvalvoja**.</span><span class="sxs-lookup"><span data-stu-id="27834-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="27834-120">c.</span><span class="sxs-lookup"><span data-stu-id="27834-120">c.</span></span> <span data-ttu-id="27834-121">Laajenna vasemmassa alakulmassa **Järjestelmänvalvoja** ja valitse **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="27834-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="27834-122">D.</span><span class="sxs-lookup"><span data-stu-id="27834-122">d.</span></span> <span data-ttu-id="27834-123">Siirry **Protection**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="27834-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="27834-124">E.</span><span class="sxs-lookup"><span data-stu-id="27834-124">e.</span></span> <span data-ttu-id="27834-125">Valitse toimialue ja valitse sitten **Ota käyttöön** tämän **toimialueen allekirjoita-viesteissä DKIM-allekirjoituksilla**.</span><span class="sxs-lookup"><span data-stu-id="27834-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="27834-126">Toista tämä vaihe jokaisen mukautetun toimialueen kohdalla.</span><span class="sxs-lookup"><span data-stu-id="27834-126">Repeat this step for each custom domain.</span></span>
