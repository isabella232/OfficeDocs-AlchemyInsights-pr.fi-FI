---
title: DLP ei toimi odotetulla tavalla
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707807"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="531e3-102">DLP ei toimi odotetulla tavalla</span><span class="sxs-lookup"><span data-stu-id="531e3-102">DLP not working as expected</span></span>

<span data-ttu-id="531e3-103">**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="531e3-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="531e3-104">**DLP:n määrittäminen**</span><span class="sxs-lookup"><span data-stu-id="531e3-104">**Setting up DLP**</span></span>

<span data-ttu-id="531e3-105">Onko Office 365:n tietojen menetyksen estämisessä **(DLP)** ongelmia, jotka eivät toimi odotetulla tavalla?</span><span class="sxs-lookup"><span data-stu-id="531e3-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="531e3-106">Jos on, varmista, että **DLP-käytäntö** on määritetty oikein ja että tietosi sisältävät sen, mitä **DLP-käytäntö** etsii, kun sitä arvioidaan.</span><span class="sxs-lookup"><span data-stu-id="531e3-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="531e3-107">DLP-käytännöt mahdollistavat luottamuksellisten tietojen tunnistamisen ja suojaamisen organisaatiossasi.</span><span class="sxs-lookup"><span data-stu-id="531e3-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="531e3-108">Jos haluat määrittää DLP-käytäntöjä, käytä näitä [tietoja.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)</span><span class="sxs-lookup"><span data-stu-id="531e3-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="531e3-109">**Mitä DLP-käytännöt näyttävät**</span><span class="sxs-lookup"><span data-stu-id="531e3-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="531e3-110">Kun tietoturva- ja yhteensopivuuskeskuksissa käytetään sisäänrakennettuja luottamuksellisia tietotyyppejä, **DLP-käytännöt** etsivät tiettyjä kaavoja ja elementtejä tunnistaessaan näitä luottamuksellisia tyyppejä.</span><span class="sxs-lookup"><span data-stu-id="531e3-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="531e3-111">**Sisäänrakennettu luottamuksellisten tietojen tyypit**</span><span class="sxs-lookup"><span data-stu-id="531e3-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="531e3-112">Tietoja valmiista luottamuksellisista tyypeistä ja siitä, mitä DLP-käytäntö etsii tunnistaessaan Luottamukselliset-tyypin, on seuraavassa kohdassa: Mitä luottamukselliset tietotyypit [etsivät.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="531e3-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="531e3-113">**Mukautetut luottamukselliset tietotyypit**</span><span class="sxs-lookup"><span data-stu-id="531e3-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="531e3-114">Jos yrität luoda mukautettuja luottamuksellisia tietotyyppejä, saat seuraavan artikkelin avulla lisätietoja mukautetun luottamuksellisen tietotyypin luosta: Mukautetun [luottamuksellisen tietotyypin luominen.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="531e3-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="531e3-115">**DLP-käytännön testaaminen**</span><span class="sxs-lookup"><span data-stu-id="531e3-115">**Test a DLP policy**</span></span>

<span data-ttu-id="531e3-116">Voit testata tietoja valmiilla tai mukautetuilla luottamuksellisilla  tietotyypeillä Käyttämällä Testityyppi-vaihtoehtoa Luokitukset   >  **luottamukselliset tietotyypit -kohdassa.**</span><span class="sxs-lookup"><span data-stu-id="531e3-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="531e3-117">Lisätietoja on kohdassa Mukautettujen [luottamuksellisten tietotyyppien testaaminen.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="531e3-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="531e3-118">**Raportit**</span><span class="sxs-lookup"><span data-stu-id="531e3-118">**Reports**</span></span>
  
- <span data-ttu-id="531e3-119">DLP-raporttien avulla saat [luottamuksellisia tietoja.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="531e3-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="531e3-120">Voit tarkastella tapahtuman yksityiskohtaisia tietoja [tapahtumaraportin avulla.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="531e3-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
