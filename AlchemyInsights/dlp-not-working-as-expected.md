---
title: DLP ei toimi odotetusti
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: 940169c0edf638b5086d70cc275049f01dcff3cf
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/08/2020
ms.locfileid: "42977435"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="670d9-102">DLP ei toimi odotetusti</span><span class="sxs-lookup"><span data-stu-id="670d9-102">DLP not working as expected</span></span>

<span data-ttu-id="670d9-103">**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="670d9-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="670d9-104">**DLP:n määrittäminen**</span><span class="sxs-lookup"><span data-stu-id="670d9-104">**Setting up DLP**</span></span>

<span data-ttu-id="670d9-105">Onko Office 365:n **DLP(Data Loss Prevention)** -ongelma, joka ei toimi odotetulla tavalla?</span><span class="sxs-lookup"><span data-stu-id="670d9-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="670d9-106">Jos näin on, varmista, että **DLP-käytäntö** on määritetty oikein ja että tiedot sisältävät sen, mitä **DLP-käytäntö** etsii, kun niitä arvioidaan.</span><span class="sxs-lookup"><span data-stu-id="670d9-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="670d9-107">DLP-käytäntöjen avulla voit tunnistaa ja suojata organisaation arkaluonteisia tietoja.</span><span class="sxs-lookup"><span data-stu-id="670d9-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="670d9-108">Voit määrittää DLP-käytännöt [tässä .](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)</span><span class="sxs-lookup"><span data-stu-id="670d9-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="670d9-109">**Mitä DLP-käytännöt etsivät**</span><span class="sxs-lookup"><span data-stu-id="670d9-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="670d9-110">Kun käytät **sisäisiä arkaluonteisia tietotyyppejä** Office 365:n suojaus- ja yhteensopivuuskeskuksessa, DLP-käytännöt etsivät tiettyjä malleja ja elementtejä, kun havaitset nämä arkaluonteiset tyypit.</span><span class="sxs-lookup"><span data-stu-id="670d9-110">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="670d9-111">**Sisäiset arkaluonteiset tietotyypit**</span><span class="sxs-lookup"><span data-stu-id="670d9-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="670d9-112">Lisätietoja sisäisistä arkaluonteisista tyypeistä ja siitä, mitä DLP-käytäntö etsii herkän tyypin havaitsemisessa, on kohdassa: [Mitä arkaluonteisia tietotyyppejä etsitään](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="670d9-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="670d9-113">**Mukautetut arkaluonteiset tietotyypit**</span><span class="sxs-lookup"><span data-stu-id="670d9-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="670d9-114">Jos yrität luoda mukautettuja arkaluonteisia tietotyyppejä, saat lisätietoja mukautetun arkaluonteisen tyypin luomisesta seuraavasta artikkelista: [Mukautetun arkaluonteisen tietotyypin luominen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="670d9-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="670d9-115">**DLP-käytännön testaaminen**</span><span class="sxs-lookup"><span data-stu-id="670d9-115">**Test a DLP policy**</span></span>

<span data-ttu-id="670d9-116">Jos haluat testata tietoja valmiilla tai mukautetulla arkaluonteisella tietotyypillä, käytä **Luokitusten** > **arkaluonteiset tietotyypit**-kohdan **Testaa tyyppi** -vaihtoehtoa.</span><span class="sxs-lookup"><span data-stu-id="670d9-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="670d9-117">Lisätietoja on kohdassa [Mukautettujen arkaluonteisten tietotyyppien testaaminen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="670d9-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="670d9-118">**Raportit**</span><span class="sxs-lookup"><span data-stu-id="670d9-118">**Reports**</span></span>
  
- <span data-ttu-id="670d9-119">Saat arkaluonteisten tietojen kävijätietoja [DLP-raporttien avulla.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="670d9-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="670d9-120">Katso tapahtuman tarkat tiedot [tapahtumaraportin](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)avulla .</span><span class="sxs-lookup"><span data-stu-id="670d9-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
