---
title: DLP sääntö SSN ei toimi
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
ms.openlocfilehash: 5af843c2b70b5b2e1aaf82c9f01356546929d840
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43788699"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="a9d51-102">DLP-ongelmat sosiaaliturvanumeroissa</span><span class="sxs-lookup"><span data-stu-id="a9d51-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="a9d51-103">**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="a9d51-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="a9d51-104">**DLP-ongelmat ssns**</span><span class="sxs-lookup"><span data-stu-id="a9d51-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="a9d51-105">Onko sinulla ongelmia **DLP (Data Loss Prevention) -toiminnon kanssa,** joka ei toimi **sosiaaliturvatunnuksen (SSN)** sisältävän sisällön kanssa, kun käytät arkaluonteista tietotyyppiä Microsoft 365:ssä?</span><span class="sxs-lookup"><span data-stu-id="a9d51-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="a9d51-106">Jos näin on, varmista, että sisältö sinetaan tarvittavat tiedot siitä, mitä DLP-käytäntö etsii.</span><span class="sxs-lookup"><span data-stu-id="a9d51-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="a9d51-107">Esimerkiksi SSN-käytännölle, jonka luotettavuustaso on 85 %, arvioidaan seuraavat tiedot, ja ne on tunnistettava, jotta sääntö käynnistyy:</span><span class="sxs-lookup"><span data-stu-id="a9d51-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="a9d51-108">**[Muoto:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 numeroa, jotka voivat olla muotoiltutai muotoilematon kuvio</span><span class="sxs-lookup"><span data-stu-id="a9d51-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="a9d51-109">**[Mallineule:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Neljä toimintoa etsii ssns neljässä eri malleja:</span><span class="sxs-lookup"><span data-stu-id="a9d51-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="a9d51-110">Func_ssn etsii ssn-nijät, joiden muotoilu on ennen vuoden 2011 vahvaa ja jotka on muotoiltu viivoilla tai välilyönneillä (ddd-dd-dddd OR ddd dd ddddd)</span><span class="sxs-lookup"><span data-stu-id="a9d51-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="a9d51-111">Func_unformatted_ssn löytää ssn-nijät, joiden vahva muotoilu on ennen vuotta 2011 ja joita ei ole muotoiltu yhdeksäksi peräkkäiseksi numeroksi (dddddddd)</span><span class="sxs-lookup"><span data-stu-id="a9d51-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="a9d51-112">Func_randomized_formatted_ssn etsii vuoden 2011 jälkeisiä ssn-naatteja, jotka on muotoiltu viivoilla tai välilyönneillä (ddd-dd-ddd OR ddd dd ddddd)</span><span class="sxs-lookup"><span data-stu-id="a9d51-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="a9d51-113">Func_randomized_unformatted_ssn löytää vuoden 2011 jälkeiset ssnit, joita ei ole muotoiltu yhdeksäksi peräkkäiseksi numeroksi (dddddddd)</span><span class="sxs-lookup"><span data-stu-id="a9d51-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="a9d51-114">**[Tarkistussumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ei, ei ole Checksumia.</span><span class="sxs-lookup"><span data-stu-id="a9d51-114">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="a9d51-115">**[Määritelmä:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP-käytäntö on 85 %: n varma siitä, että se on havainnut tämäntyyppisiä arkaluonteisia tietoja, jos 300 merkin etäisyydellä:</span><span class="sxs-lookup"><span data-stu-id="a9d51-115">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="a9d51-116">Toiminto [Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) etsii kaavaa vastaavaa sisältöä.</span><span class="sxs-lookup"><span data-stu-id="a9d51-116">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="a9d51-117">[Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) avainsana löytyy.</span><span class="sxs-lookup"><span data-stu-id="a9d51-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="a9d51-118">Avainsanoja ovat esimerkiksi *sosiaaliturva, sosiaaliturva#, Soc Sec ,SSN* .</span><span class="sxs-lookup"><span data-stu-id="a9d51-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="a9d51-119">Esimerkiksi seuraava esimerkki käynnistäisi DLP SSN -käytännön: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="a9d51-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="a9d51-120">Lisätietoja siitä, mitä sisällön ssn-nimiselle tunnistettaviksi tarvitaan, on tämän artikkelin seuraavassa osassa: [Mitä arkaluonteiset tietotyypit etsivät ssn-verkkoja](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="a9d51-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="a9d51-121">Toisen sisäisen arkaluonteisen tietotyypin avulla on seuraavassa artikkelissa tietoja siitä, mitä muille tyypeille tarvitaan: [Mitä arkaluonteiset tietotyypit etsivät](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="a9d51-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  