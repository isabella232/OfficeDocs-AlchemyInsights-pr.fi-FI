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
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932619"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="3b7b5-102">DLP ei toimi odotetusti</span><span class="sxs-lookup"><span data-stu-id="3b7b5-102">DLP not working as expected</span></span>

<span data-ttu-id="3b7b5-103">**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan.</span><span class="sxs-lookup"><span data-stu-id="3b7b5-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="3b7b5-104">Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut.</span><span class="sxs-lookup"><span data-stu-id="3b7b5-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="3b7b5-105">Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.</span><span class="sxs-lookup"><span data-stu-id="3b7b5-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="3b7b5-106">Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan.</span><span class="sxs-lookup"><span data-stu-id="3b7b5-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="3b7b5-107">Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina.</span><span class="sxs-lookup"><span data-stu-id="3b7b5-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="3b7b5-108">Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.</span><span class="sxs-lookup"><span data-stu-id="3b7b5-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="3b7b5-109">**DLP:n määrittäminen**</span><span class="sxs-lookup"><span data-stu-id="3b7b5-109">**Setting up DLP**</span></span>

<span data-ttu-id="3b7b5-110">Onko Office 365:n **DLP(Data Loss Prevention)** -ongelma, joka ei toimi odotetulla tavalla?</span><span class="sxs-lookup"><span data-stu-id="3b7b5-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="3b7b5-111">Jos näin on, varmista, että **DLP-käytäntö** on määritetty oikein ja että tiedot sisältävät sen, mitä **DLP-käytäntö** etsii, kun niitä arvioidaan.</span><span class="sxs-lookup"><span data-stu-id="3b7b5-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="3b7b5-112">DLP-käytäntöjen avulla voit tunnistaa ja suojata organisaation arkaluonteisia tietoja.</span><span class="sxs-lookup"><span data-stu-id="3b7b5-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="3b7b5-113">Voit määrittää DLP-käytännöt [tässä .](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)</span><span class="sxs-lookup"><span data-stu-id="3b7b5-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="3b7b5-114">**Mitä DLP-käytännöt etsivät**</span><span class="sxs-lookup"><span data-stu-id="3b7b5-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="3b7b5-115">Kun käytät **sisäisiä arkaluonteisia tietotyyppejä** Office 365:n suojaus- ja yhteensopivuuskeskuksessa, DLP-käytännöt etsivät tiettyjä malleja ja elementtejä, kun havaitset nämä arkaluonteiset tyypit.</span><span class="sxs-lookup"><span data-stu-id="3b7b5-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="3b7b5-116">**Sisäiset arkaluonteiset tietotyypit**</span><span class="sxs-lookup"><span data-stu-id="3b7b5-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="3b7b5-117">Lisätietoja sisäisistä arkaluonteisista tyypeistä ja siitä, mitä DLP-käytäntö etsii herkän tyypin havaitsemisessa, on kohdassa: [Mitä arkaluonteisia tietotyyppejä etsitään](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="3b7b5-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="3b7b5-118">**Mukautetut arkaluonteiset tietotyypit**</span><span class="sxs-lookup"><span data-stu-id="3b7b5-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="3b7b5-119">Jos yrität luoda mukautettuja arkaluonteisia tietotyyppejä, saat lisätietoja mukautetun arkaluonteisen tyypin luomisesta seuraavasta artikkelista: [Mukautetun arkaluonteisen tietotyypin luominen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="3b7b5-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="3b7b5-120">**DLP-käytännön testaaminen**</span><span class="sxs-lookup"><span data-stu-id="3b7b5-120">**Test a DLP policy**</span></span>

<span data-ttu-id="3b7b5-121">Jos haluat testata tietoja valmiilla tai mukautetulla arkaluonteisella tietotyypillä, käytä **Luokitusten** > **arkaluonteiset tietotyypit**-kohdan **Testaa tyyppi** -vaihtoehtoa.</span><span class="sxs-lookup"><span data-stu-id="3b7b5-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="3b7b5-122">Lisätietoja on kohdassa [Mukautettujen arkaluonteisten tietotyyppien testaaminen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="3b7b5-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="3b7b5-123">**Raportit**</span><span class="sxs-lookup"><span data-stu-id="3b7b5-123">**Reports**</span></span>
  
- <span data-ttu-id="3b7b5-124">Saat arkaluonteisten tietojen kävijätietoja [DLP-raporttien avulla.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="3b7b5-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="3b7b5-125">Katso tapahtuman tarkat tiedot [tapahtumaraportin](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)avulla .</span><span class="sxs-lookup"><span data-stu-id="3b7b5-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
