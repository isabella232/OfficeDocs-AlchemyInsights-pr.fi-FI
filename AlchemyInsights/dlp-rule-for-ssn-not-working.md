---
title: DLP-sääntö ei toimi SSN-palvelussa
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679366"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="eff8a-102">DLP-ongelmat Sosiaaliturvanumeroissa</span><span class="sxs-lookup"><span data-stu-id="eff8a-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="eff8a-103">**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="eff8a-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="eff8a-104">**DLP-ongelmat SSN:llä**</span><span class="sxs-lookup"><span data-stu-id="eff8a-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="eff8a-105">Onko sinulla ongelmia **tietojen menetyksen estämisen (DLP)** kanssa, joka ei toimi, jos sisältö sisältää **SOSIAALITURVANUMERON (SSN)** , kun Microsoft 365-palvelussa käytetään arkaluonteista tieto tyyppiä?</span><span class="sxs-lookup"><span data-stu-id="eff8a-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="eff8a-106">Varmista, että sisältö sisältää tarvittavat tiedot siitä, mitä DLP-käytäntöä etsitään.</span><span class="sxs-lookup"><span data-stu-id="eff8a-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="eff8a-107">Esimerkiksi SSN-käytännölle, jonka luotettavuus taso on 85%, lasketaan seuraavat ja on havaittu, että sääntö käynnistetään:</span><span class="sxs-lookup"><span data-stu-id="eff8a-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="eff8a-108">**[Muoto:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 numeroa, jotka voivat olla muotoiltuna tai muotoilemattomana kuviona</span><span class="sxs-lookup"><span data-stu-id="eff8a-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="eff8a-109">**[Malli neule:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Neljä funktiota näyttävät SSN:t neljässä eri kuvioissa:</span><span class="sxs-lookup"><span data-stu-id="eff8a-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="eff8a-110">Func_ssn löytää SSNS:n, jossa on ennen 2011 vahvaa muotoilua, joka on muotoiltu katko viivoilla tai väli lyönneillä (DDD-DD-dddd tai TDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="eff8a-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="eff8a-111">Func_unformatted_ssn löytää SSN-version, jossa on ennen 2011 vahvaa muotoilua, jonka muotoilu on yhdeksän peräkkäistä numeroa (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="eff8a-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="eff8a-112">Func_randomized_formatted_ssn löytää post-2011 SSN-merkit, jotka on muotoutunut viivoilla tai väli lyönneillä (DDD-DD-dddd tai TDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="eff8a-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="eff8a-113">Func_randomized_unformatted_ssn hakee post-2011-SSN-tunnukset, jotka ovat muotoilemattomia yhdeksässä peräkkäisessä numerona (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="eff8a-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="eff8a-114">**[Tarkistus summa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ei, tarkistus summaa ei ole</span><span class="sxs-lookup"><span data-stu-id="eff8a-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="eff8a-115">**[Määritelmä:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP-käytännöllä on 85% varma, että se havaitsee tämän tyyppisiä tietoja, jos se on 300-merkin lähellä:</span><span class="sxs-lookup"><span data-stu-id="eff8a-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="eff8a-116">[Funktio Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) löytää kaavaa vastaavaa sisältöä.</span><span class="sxs-lookup"><span data-stu-id="eff8a-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="eff8a-117">[Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) avain sana löytyy.</span><span class="sxs-lookup"><span data-stu-id="eff8a-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="eff8a-118">Esimerkkejä avain sanoista ovat:  *sosiaaliturva, sosiaaliturva #, SOC SEC, SSN*  .</span><span class="sxs-lookup"><span data-stu-id="eff8a-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="eff8a-119">Esimerkiksi seuraava esimerkki käynnistäisi DLP SSN-käytäntöä: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="eff8a-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="eff8a-120">Jos haluat lisä tietoja siitä, mitä SSN:ltä edellytetään sisällölle, Lue tämän artikkelin seuraava osio: [mitä luottamukselliset tieto tyypit etsivät SSN:stä](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="eff8a-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="eff8a-121">Jos käytät erilaista sisäistä arkaluonteista tieto tyyppiä, Katso lisä tietoja muista tieto tyypeistä, jotka ovat tarpeen: [mitä luottamukselliset tieto tyypit](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) etsivät</span><span class="sxs-lookup"><span data-stu-id="eff8a-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  