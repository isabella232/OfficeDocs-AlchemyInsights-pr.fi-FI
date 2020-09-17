---
title: Setup DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808704"
---
# <a name="setup-dkim"></a><span data-ttu-id="0baf1-102">Setup DKIM</span><span class="sxs-lookup"><span data-stu-id="0baf1-102">Setup DKIM</span></span>

<span data-ttu-id="0baf1-103">Microsoft 365: n mukautettujen toimi alueiden DKIM-määrityksen täydelliset ohjeet ovat [täällä](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="0baf1-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="0baf1-104">Sinun on luotava **kullekin** mukautetulle toimi alueelle **kaksi** DKIM CNAME-tietuetta toimi alueen DNS-isännöinti palvelussa (yleensä toimi alueen rekisteröinti palvelu).</span><span class="sxs-lookup"><span data-stu-id="0baf1-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="0baf1-105">Esimerkiksi contoso.com ja fourthcoffee.com vaativat neljä DKIM CNAME-tietuetta: kaksi contoso.com ja kaksi fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="0baf1-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="0baf1-106">**Kunkin** mukautetun toimi alueen DKIM CNAME-tietueet käyttävät seuraavia muotoiluja:</span><span class="sxs-lookup"><span data-stu-id="0baf1-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="0baf1-107">**Isäntä nimi**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="0baf1-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="0baf1-108">**Osoittaa osoitteen tai arvon**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="0baf1-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="0baf1-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="0baf1-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="0baf1-110">**Isäntä nimi**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="0baf1-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="0baf1-111">**Osoittaa osoitteen tai arvon**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="0baf1-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="0baf1-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="0baf1-112">**TTL**: 3600</span></span>

   <span data-ttu-id="0baf1-113">\<DomainGUID\> on `.mail.protection.outlook.com` mukautetun toimi alueen mukautetun MX-tietueen (esimerkiksi `contoso-com` toimi alueen contoso.com) vasemmalla puolella oleva teksti.</span><span class="sxs-lookup"><span data-stu-id="0baf1-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="0baf1-114">\<InitialDomain\> on toimi alue, jota käytit rekisteröityessäsi Microsoft 365-käyttöön (esimerkiksi contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="0baf1-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="0baf1-115">Kun olet luonut mukautettujen toimi alueiden CNAME-tietueet, noudata seuraavia ohjeita:</span><span class="sxs-lookup"><span data-stu-id="0baf1-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="0baf1-116">a.</span><span class="sxs-lookup"><span data-stu-id="0baf1-116">a.</span></span> <span data-ttu-id="0baf1-117">[Kirjaudu sisään Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) työpaikan tai oppi laitoksen tilillä.</span><span class="sxs-lookup"><span data-stu-id="0baf1-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="0baf1-118">b.</span><span class="sxs-lookup"><span data-stu-id="0baf1-118">b.</span></span> <span data-ttu-id="0baf1-119">Valitse vasemmasta yläkulmasta sovellusten käynnistyskuvake ja valitse **Järjestelmänvalvoja**.</span><span class="sxs-lookup"><span data-stu-id="0baf1-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="0baf1-120">c.</span><span class="sxs-lookup"><span data-stu-id="0baf1-120">c.</span></span> <span data-ttu-id="0baf1-121">Laajenna vasemmassa alakulmassa olevaa siirtymis ruudussa **järjestelmänvalvoja** -kohtaa ja valitse **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="0baf1-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="0baf1-122">d.</span><span class="sxs-lookup"><span data-stu-id="0baf1-122">d.</span></span> <span data-ttu-id="0baf1-123">Siirry kohtaan **Suojaus**-  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="0baf1-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="0baf1-124">e.</span><span class="sxs-lookup"><span data-stu-id="0baf1-124">e.</span></span> <span data-ttu-id="0baf1-125">Valitse toimi alue ja valitse sitten **Ota käyttöön** **tämän toimi alueen allekirjoita viestit DKIM-allekirjoituksilla**.</span><span class="sxs-lookup"><span data-stu-id="0baf1-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="0baf1-126">Toista tämä vaihe kunkin mukautetun toimi alueen kohdalla.</span><span class="sxs-lookup"><span data-stu-id="0baf1-126">Repeat this step for each custom domain.</span></span>
