---
title: DLP ei toimi odotetulla tavalla
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
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507475"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="c5d60-102">DLP ei toimi odotetulla tavalla</span><span class="sxs-lookup"><span data-stu-id="c5d60-102">DLP not working as expected</span></span>

<span data-ttu-id="c5d60-103">**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="c5d60-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="c5d60-104">**DLP:n määrittäminen**</span><span class="sxs-lookup"><span data-stu-id="c5d60-104">**Setting up DLP**</span></span>

<span data-ttu-id="c5d60-105">Onko sinulla ongelmia **Tietojen menetyksen estämisessä (DLP)** Office 365:ssä, joka ei toimi odotetulla tavalla?</span><span class="sxs-lookup"><span data-stu-id="c5d60-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="c5d60-106">Jos näin on, varmista, että **DLP-käytäntö** on määritetty oikein ja että tietosi sisältävät sen, mitä **DLP-käytäntö** etsii, kun sitä arvioidaan.</span><span class="sxs-lookup"><span data-stu-id="c5d60-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="c5d60-107">DLP-käytäntöjen avulla voit tunnistaa ja suojata organisaation arkaluonteisia tietoja.</span><span class="sxs-lookup"><span data-stu-id="c5d60-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="c5d60-108">Voit määrittää DLP-käytännöt tässä [tiedoissa.](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)</span><span class="sxs-lookup"><span data-stu-id="c5d60-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="c5d60-109">**Mitä DLP-käytännöt etsivät**</span><span class="sxs-lookup"><span data-stu-id="c5d60-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="c5d60-110">Kun käytät tietoturva- ja yhteensopivuuskeskusten **sisäisiä arkaluonteisia tietotyyppejä, DLP-käytännöt** etsivät tiettyjä malleja ja elementtejä näitä arkaluonteisia tyyppejä havaittaessa.</span><span class="sxs-lookup"><span data-stu-id="c5d60-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="c5d60-111">**Sisäiset arkaluonteiset tietotyypit**</span><span class="sxs-lookup"><span data-stu-id="c5d60-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="c5d60-112">Lisätietoja sisäisistä arkaluonteisista tyypeistä ja siitä, mitä DLP-käytäntö etsii arkaluonteisen tyypin tunnistamisessa, on ohjeaiheessa [Mitä arkaluonteiset tietotyypit etsivät](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="c5d60-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="c5d60-113">**Mukautetut arkaluonteiset tietotyypit**</span><span class="sxs-lookup"><span data-stu-id="c5d60-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="c5d60-114">Jos yrität luoda mukautettuja arkaluonteisia tietotyyppejä, käytä seuraavaa artikkelia mukautetun arkaluonteisen tyypin luomisesta: [Mukautetun arkaluonteisen tietotyypin luominen](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="c5d60-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="c5d60-115">**DLP-käytännön testaaminen**</span><span class="sxs-lookup"><span data-stu-id="c5d60-115">**Test a DLP policy**</span></span>

<span data-ttu-id="c5d60-116">Jos haluat testata tietoja valmiilla tai mukautetuilla arkaluonteisilla tietotyypeillä, käytä **Luokitusten** **Classifications**  >  **arkaluonteiset tietotyypit**-kohdan Testaa tyyppi -vaihtoehtoa.</span><span class="sxs-lookup"><span data-stu-id="c5d60-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="c5d60-117">Lisätietoja on kohdassa [Mukautettujen arkaluonteisten tietotyyppien testaaminen](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="c5d60-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="c5d60-118">**Raportit**</span><span class="sxs-lookup"><span data-stu-id="c5d60-118">**Reports**</span></span>
  
- <span data-ttu-id="c5d60-119">Saat arkaluonteisia tietoja [DLP-raporttien avulla.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="c5d60-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="c5d60-120">Katso tapahtuman tarkat tiedot [tapahtumaraportin](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)avulla .</span><span class="sxs-lookup"><span data-stu-id="c5d60-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
