---
title: DLP ei toimi odotetulla tavalla
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
ms.openlocfilehash: 1ea457bd69e7d545cf761a0be849695738b19d8b
ms.sourcegitcommit: d6ea6f4456a582559f27b34c0b9455a86a8e61f1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/31/2019
ms.locfileid: "35941065"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="ec74b-102">DLP ei toimi odotetulla tavalla</span><span class="sxs-lookup"><span data-stu-id="ec74b-102">DLP not working as expected</span></span>

<span data-ttu-id="ec74b-103">Sinulla on ongelmia **Tietojen menetyksen ehkäisyyn (DLP)** ei toimi odotetulla tavalla Office 365: ssä?</span><span class="sxs-lookup"><span data-stu-id="ec74b-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="ec74b-104">Jos näin on, varmista, että **DLP-käytäntö** on määritetty oikein ja että tiedot sisältävät mitä **DLP käytännön** etsii kun on arvioitava.</span><span class="sxs-lookup"><span data-stu-id="ec74b-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="ec74b-105">**DLP määrittäminen**</span><span class="sxs-lookup"><span data-stu-id="ec74b-105">**Setting up DLP**</span></span>
  
<span data-ttu-id="ec74b-106">DLP-käytäntöjen avulla voit tunnistaa ja suojaa organisaatiosi luottamukselliset tiedot.</span><span class="sxs-lookup"><span data-stu-id="ec74b-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="ec74b-107">DLP-käytäntöjen asetukset, käytä tiedot [tähän](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="ec74b-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="ec74b-108">**Etsi mitä DLP-käytännöt**</span><span class="sxs-lookup"><span data-stu-id="ec74b-108">**What DLP policies look for**</span></span>
  
<span data-ttu-id="ec74b-109">Käytettäessä **tyypit sisäisiä luottamuksellisia tietoja** Office 365: n tietoturvan ja määritystenmukaisuuden center DLP käytännöt näyttää talousjärjestelmän ja osien tunnistaminen tällaisia arkaluonteisia.</span><span class="sxs-lookup"><span data-stu-id="ec74b-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="ec74b-110">**Sisäänrakennettu luottamuksellisten tietojen tyypit**</span><span class="sxs-lookup"><span data-stu-id="ec74b-110">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="ec74b-111">Herkkä valmiiksi määritetyt tyypit ja mitä käytännön DLP etsii kun tunnistaminen herkkä laji, Lisätietoja: [Etsi mitä luottamuksellisten tietojen tyypit](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="ec74b-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="ec74b-112">**Mukautettu luottamuksellisten tietojen tyypit**</span><span class="sxs-lookup"><span data-stu-id="ec74b-112">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="ec74b-113">Jos yrität luoda mukautetun luottamuksellisia tietoja, käytä seuraavassa artikkelissa luodaan mukautettu luottamuksellisia tietoja: [Luo mukautetun luottamuksellisten tietojen tyyppi](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="ec74b-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="ec74b-114">**DLP-käytännön testi**</span><span class="sxs-lookup"><span data-stu-id="ec74b-114">**Test a DLP policy**</span></span>

<span data-ttu-id="ec74b-115">Testaa tietosi valmiiseen tai mukautettuun luottamuksellisten tietojen tyypin kanssa, käytä **testityyppi** asetuksen **luokitusten** > **tyypit luottamuksellisia tietoja**.</span><span class="sxs-lookup"><span data-stu-id="ec74b-115">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="ec74b-116">Lisätietoja [mukautetun luottamuksellisten tietojen tyyppejä](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="ec74b-116">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="ec74b-117">**Raportit**</span><span class="sxs-lookup"><span data-stu-id="ec74b-117">**Reports**</span></span>
  
- <span data-ttu-id="ec74b-118">Saada luottamuksellisia tietoja ja näkemyksiä [Raportit DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="ec74b-118">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="ec74b-119">Katso tapahtuma [Tapaus raportin](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)tiedot.</span><span class="sxs-lookup"><span data-stu-id="ec74b-119">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
