---
title: DLP-sääntö, jos SSN ei toimi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507367"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="46f3f-102">DLP-ongelmat sosiaaliturvatunnusten kanssa</span><span class="sxs-lookup"><span data-stu-id="46f3f-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="46f3f-103">**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="46f3f-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="46f3f-104">**DLP-ongelmat SSN:ssä**</span><span class="sxs-lookup"><span data-stu-id="46f3f-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="46f3f-105">Onko sinulla ongelmia, kun **tietoja katoamisen estämisessä (DLP)** ei ole käytössä sisältöä, joka sisältää **SSN:n (SSN),** kun käytät microsoft 365:n arkaluonteista tietotyyppiä?</span><span class="sxs-lookup"><span data-stu-id="46f3f-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="46f3f-106">Jos näin on, varmista, että sisältö sisältää tarvittavat tiedot siitä, mitä DLP-käytäntö etsii.</span><span class="sxs-lookup"><span data-stu-id="46f3f-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="46f3f-107">Esimerkiksi SSN-käytännössä, jonka luotettavuustaso on 85 %, arvioidaan seuraavat tiedot, jotka on tunnistettava, jotta sääntö käynnistyisi:</span><span class="sxs-lookup"><span data-stu-id="46f3f-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="46f3f-108">**[Muoto:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 numeroa, jotka voivat olla muotoiltu tai muotoilematon kuvio</span><span class="sxs-lookup"><span data-stu-id="46f3f-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="46f3f-109">**[Mallineule:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Neljä toimintoa etsiä SSNs neljä eri malleja:</span><span class="sxs-lookup"><span data-stu-id="46f3f-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="46f3f-110">Func_ssn etsii SSN-nit, joiden ennen 2011 -muotoista muotoilua on muotoiltu viivoilla tai välilyönneillä (ddd-dd-dddd OR ddd ddddd)</span><span class="sxs-lookup"><span data-stu-id="46f3f-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="46f3f-111">Func_unformatted_ssn etsii SSN-nit, joiden ennen vuotta 2011 on vahva muotoilu ja jotka eivät ole muotoiltu yhdeksäksi peräkkäiseksi numeroksi (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="46f3f-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="46f3f-112">Func_randomized_formatted_ssn etsii vuoden 2011 jälkeisiä SSN-nistoja, jotka on muotoiltu vikoilla tai välilyönneillä (ddd-dd-dddd OR ddd ddddd)</span><span class="sxs-lookup"><span data-stu-id="46f3f-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="46f3f-113">Func_randomized_unformatted_ssn etsii vuoden 2011 jälkeisiä SSN-numeroita, jotka ovat muotoilemattomia yhdeksäksi peräkkäiseksi numeroksi (dddddddd)</span><span class="sxs-lookup"><span data-stu-id="46f3f-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="46f3f-114">**[Tarkistussumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ei, tarkistussummaa ei ole.</span><span class="sxs-lookup"><span data-stu-id="46f3f-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="46f3f-115">**[Määritelmä:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP-käytäntö on 85% varma siitä, että se on havainnut tällaisia arkaluonteisia tietoja, jos 300 merkin läheisyydessä:</span><span class="sxs-lookup"><span data-stu-id="46f3f-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="46f3f-116">[Funktio Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) etsii kuviota vastaavaa sisältöä.</span><span class="sxs-lookup"><span data-stu-id="46f3f-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="46f3f-117">Avainsana [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) löytyy.</span><span class="sxs-lookup"><span data-stu-id="46f3f-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="46f3f-118">Esimerkkejä avainsanoista ovat: *Sosiaaliturva, Sosiaaliturva#, Soc Sec, SSN* .</span><span class="sxs-lookup"><span data-stu-id="46f3f-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="46f3f-119">Esimerkiksi seuraava esimerkki käynnistäisi DLP SSN -käytännön: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="46f3f-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="46f3f-120">Lisätietoja siitä, mitä ssn-tekniikat ovat velvollisia havaitsemaan sisältöäsi varten, on seuraavassa tämän artikkelin osassa: [Mitä arkaluonteiset tietotyypit etsivät SSN-tyyppejä](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="46f3f-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="46f3f-121">Jos käytät eri sisäänrakennettua arkaluonteista tietotyyppiä, lue seuraavassa artikkelissa tietoja siitä, mitä tarvitaan muuntyyppisille [tyypeille: Mitä arkaluonteiset tietotyypit etsivät](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="46f3f-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  