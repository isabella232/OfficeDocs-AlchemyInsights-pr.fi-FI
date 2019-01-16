---
title: SSN-ei toimi DLP-sääntö
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b92d122b774d97cd2e44cc0880dc5001065b57cc
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28286489"
---
<span data-ttu-id="3e2a9-p101">Onko sinulla ongelmia kanssa **Tietojen menetyksen ehkäisyyn (DLP)** sisällön sisältävän **Henkilötunnus (SSN)** luottamuksellisten tietojen tyyppiä käytettäessä Office 365: ssä ei toimi? Jos näin on, varmista, että sisältösi on DLP-käytäntö on selvittämiseen tarvittavia tietoja.</span><span class="sxs-lookup"><span data-stu-id="3e2a9-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365? If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="3e2a9-104">Esimerkiksi määritetty 85 %: n varmuudella SSN-käytäntö, seuraavat arvioidaan ja havaittu käynnistää säännön:</span><span class="sxs-lookup"><span data-stu-id="3e2a9-104">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="3e2a9-105">**[Muoto:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 numeroa, joka voi olla muotoiltuna tai muotoilemattomana kuvio</span><span class="sxs-lookup"><span data-stu-id="3e2a9-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span> 
    
- <span data-ttu-id="3e2a9-106">**[Kuvio:](https://msconnect.microsoft.com/https:/docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Neljä Funktiot Etsi SSNs neljä eri kuviot:</span><span class="sxs-lookup"><span data-stu-id="3e2a9-106">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span> 
    
  - <span data-ttu-id="3e2a9-107">Func_ssn löytää SSNs ja pre-2011 vahva muotoilu, jotka on muotoiltu väliviivoja tai välilyöntejä (ddd-pp-dddd tai ddd pp dddd)</span><span class="sxs-lookup"><span data-stu-id="3e2a9-107">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="3e2a9-108">Func_unformatted_ssn löytää SSNs ja pre-2011 vahva muotoilu, joka on alustettu yhdeksän peräkkäistä merkkiä (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="3e2a9-108">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
  - <span data-ttu-id="3e2a9-109">Func_randomized_formatted_ssn löytää post-2011 SSNs, jotka on muotoiltu väliviivoja tai välilyöntejä (ddd-pp-dddd tai ddd pp dddd)</span><span class="sxs-lookup"><span data-stu-id="3e2a9-109">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="3e2a9-110">Func_randomized_unformatted_ssn löytää post-2011 SSNs, joka on alustettu yhdeksän peräkkäistä merkkiä (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="3e2a9-110">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
- <span data-ttu-id="3e2a9-111">**[Tarkistussumma:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ei, ei ole tarkistussumma</span><span class="sxs-lookup"><span data-stu-id="3e2a9-111">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="3e2a9-112">**[Määritelmä:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP-käytäntö on 85 % varma siitä, että se on havainnut arkaluonteisia henkilötietoja Jos läheisyydessä 300 merkkiä sisällä:</span><span class="sxs-lookup"><span data-stu-id="3e2a9-112">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="3e2a9-113">[Func_ssn-funktio](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) etsii kuviota vastaava sisältö.</span><span class="sxs-lookup"><span data-stu-id="3e2a9-113">The [function Func_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span> 
    
  - <span data-ttu-id="3e2a9-p102">- [Keyword_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) avainsana on löytynyt. Sisältää esimerkkejä avainsanat: *sosiaaliturva, sosiaaliturvan #, Soc s, SSN* . Esimerkiksi seuraava esimerkki käynnistää käytännön DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="3e2a9-p102">A keyword from [Keyword_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found. Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  . For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
    
<span data-ttu-id="3e2a9-117">Katso lisätietoja mitä tarvitaan sisällön tunnistaminen SSNs on tämän artikkelin seuraavassa osassa: [Mitä on herkkä tietotyypit etsiä SSNs](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="3e2a9-117">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="3e2a9-118">Käyttämällä erilaisia sisäisiä luottamuksellisia tietoja, seuraavasta artikkelista lisätietoja, mitä tarvitaan muissa yhteyksissä: [Etsi mitä luottamuksellisten tietojen tyypit](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="3e2a9-118">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

