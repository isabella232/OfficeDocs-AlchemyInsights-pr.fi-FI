---
title: DLP ei toimi odotetusti
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: efb4a19f345fe6b8a1e8bb72abeba4a923c05777
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704410"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="12a5e-102">DLP ei toimi odotetusti</span><span class="sxs-lookup"><span data-stu-id="12a5e-102">DLP not working as expected</span></span>

<span data-ttu-id="12a5e-103">**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="12a5e-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="12a5e-104">**DLP:n määrittäminen**</span><span class="sxs-lookup"><span data-stu-id="12a5e-104">**Setting up DLP**</span></span>

<span data-ttu-id="12a5e-105">Onko Office 365:n **DLP(Data Loss Prevention)** -ongelma, joka ei toimi odotetulla tavalla?</span><span class="sxs-lookup"><span data-stu-id="12a5e-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="12a5e-106">Jos näin on, varmista, että **DLP-käytäntö** on määritetty oikein ja että tiedot sisältävät sen, mitä **DLP-käytäntö** etsii, kun niitä arvioidaan.</span><span class="sxs-lookup"><span data-stu-id="12a5e-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="12a5e-107">DLP-käytäntöjen avulla voit tunnistaa ja suojata organisaation arkaluonteisia tietoja.</span><span class="sxs-lookup"><span data-stu-id="12a5e-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="12a5e-108">Voit määrittää DLP-käytännöt [tässä .](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)</span><span class="sxs-lookup"><span data-stu-id="12a5e-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="12a5e-109">**Mitä DLP-käytännöt etsivät**</span><span class="sxs-lookup"><span data-stu-id="12a5e-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="12a5e-110">Kun dlp-käytäntöjä käytetään suojaus- ja yhteensopivuuskeskuksissa, **dlp-käytännöt** etsivät tiettyjä malleja ja elementtejä, kun havaitset nämä arkaluonteiset tyypit.</span><span class="sxs-lookup"><span data-stu-id="12a5e-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="12a5e-111">**Sisäiset arkaluonteiset tietotyypit**</span><span class="sxs-lookup"><span data-stu-id="12a5e-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="12a5e-112">Lisätietoja sisäisistä arkaluonteisista tyypeistä ja siitä, mitä DLP-käytäntö etsii herkän tyypin havaitsemisessa, on kohdassa: [Mitä arkaluonteisia tietotyyppejä etsitään](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="12a5e-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="12a5e-113">**Mukautetut arkaluonteiset tietotyypit**</span><span class="sxs-lookup"><span data-stu-id="12a5e-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="12a5e-114">Jos yrität luoda mukautettuja arkaluonteisia tietotyyppejä, saat lisätietoja mukautetun arkaluonteisen tyypin luomisesta seuraavasta artikkelista: [Mukautetun arkaluonteisen tietotyypin luominen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="12a5e-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="12a5e-115">**DLP-käytännön testaaminen**</span><span class="sxs-lookup"><span data-stu-id="12a5e-115">**Test a DLP policy**</span></span>

<span data-ttu-id="12a5e-116">Jos haluat testata tietoja valmiilla tai mukautetulla arkaluonteisella tietotyypillä, käytä **Luokitusten** > **arkaluonteiset tietotyypit**-kohdan **Testaa tyyppi** -vaihtoehtoa.</span><span class="sxs-lookup"><span data-stu-id="12a5e-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="12a5e-117">Lisätietoja on kohdassa [Mukautettujen arkaluonteisten tietotyyppien testaaminen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="12a5e-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="12a5e-118">**Raportit**</span><span class="sxs-lookup"><span data-stu-id="12a5e-118">**Reports**</span></span>
  
- <span data-ttu-id="12a5e-119">Saat arkaluonteisten tietojen kävijätietoja [DLP-raporttien avulla.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="12a5e-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="12a5e-120">Katso tapahtuman tarkat tiedot [tapahtumaraportin](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)avulla .</span><span class="sxs-lookup"><span data-stu-id="12a5e-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
