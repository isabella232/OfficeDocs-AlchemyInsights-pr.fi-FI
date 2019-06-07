---
title: 'Asennus DKIM Office 365: ssä'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765033"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="4f521-102">Asennus DKIM Office 365: ssä</span><span class="sxs-lookup"><span data-stu-id="4f521-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="4f521-103">DKIM määrittäminen Office 365: ssä mukautetut toimialueet ovat täydelliset ohjeet [tähän](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="4f521-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="4f521-104">**Kutakin** mukautettua toimialuetta täytyy luoda **kaksi** DKIM CNAME-tietueita toimialueen DNS-sivustotilapalvelun (yleensä toimialueen registrar).</span><span class="sxs-lookup"><span data-stu-id="4f521-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="4f521-105">Esimerkiksi contoso.com ja fourthcoffee.com vaativat neljä DKIM CNAME-tietueet: contoso.com ja kaksi fourthcoffee.com, kaksi.</span><span class="sxs-lookup"><span data-stu-id="4f521-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="4f521-106">**Kutakin** mukautettua toimialuetta DKIM CNAME-tietueita käytetään seuraavissa muodoissa:</span><span class="sxs-lookup"><span data-stu-id="4f521-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="4f521-107">**Isännän nimi**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="4f521-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="4f521-108">**Osoite tai arvo viittaa**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="4f521-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="4f521-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="4f521-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="4f521-110">**Isännän nimi**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="4f521-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="4f521-111">**Osoite tai arvo viittaa**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="4f521-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="4f521-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="4f521-112">**TTL**: 3600</span></span>

   <span data-ttu-id="4f521-113">\<DomainGUID\> on teksti vasemmalla puolella `.mail.protection.outlook.com` mukautetut MX-tietueen mukautetun toimialueen (esimerkiksi `contoso-com` , toimialueen contoso.com).</span><span class="sxs-lookup"><span data-stu-id="4f521-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="4f521-114">\<InitialDomain\> on toimialue, jota käytit Kun rekisteröidyit Office 365 (esimerkiksi contoso.onmicrosoft.com) varten.</span><span class="sxs-lookup"><span data-stu-id="4f521-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="4f521-115">Kun olet luonut CNAME-tietueet, mukautettujen toimialueiden, toimimalla seuraavien ohjeiden mukaan:</span><span class="sxs-lookup"><span data-stu-id="4f521-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="4f521-116">a.</span><span class="sxs-lookup"><span data-stu-id="4f521-116">a.</span></span> <span data-ttu-id="4f521-117">[Kirjaudu Office 365:een](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) antamalla työpaikan tai oppilaitoksen tili.</span><span class="sxs-lookup"><span data-stu-id="4f521-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="4f521-118">b.</span><span class="sxs-lookup"><span data-stu-id="4f521-118">b.</span></span> <span data-ttu-id="4f521-119">Valitse vasemmasta yläkulmasta sovellusten käynnistyskuvake ja valitse **Järjestelmänvalvoja**.</span><span class="sxs-lookup"><span data-stu-id="4f521-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="4f521-120">c.</span><span class="sxs-lookup"><span data-stu-id="4f521-120">c.</span></span> <span data-ttu-id="4f521-121">Vasemmassa siirtymispalkissa Laajenna **Admin** ja valitse **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="4f521-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="4f521-122">d.</span><span class="sxs-lookup"><span data-stu-id="4f521-122">d.</span></span> <span data-ttu-id="4f521-123">Siirry **Suojaa** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="4f521-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="4f521-124">e.</span><span class="sxs-lookup"><span data-stu-id="4f521-124">e.</span></span> <span data-ttu-id="4f521-125">Valitse toimialue ja valitse sitten **merkki**viesteissä DKIM-allekirjoituksia sisältävien tämän toimialueen **käyttöön** .</span><span class="sxs-lookup"><span data-stu-id="4f521-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="4f521-126">Toista tämä vaihe kunkin mukautetun toimialueen.</span><span class="sxs-lookup"><span data-stu-id="4f521-126">Repeat this step for each custom domain.</span></span>
