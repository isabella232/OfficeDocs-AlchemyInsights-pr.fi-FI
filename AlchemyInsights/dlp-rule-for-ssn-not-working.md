---
title: DLP sääntö SSN ei toimi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932518"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="969bc-102">DLP-ongelmat sosiaaliturvanumeroissa</span><span class="sxs-lookup"><span data-stu-id="969bc-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="969bc-103">**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan.</span><span class="sxs-lookup"><span data-stu-id="969bc-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="969bc-104">Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut.</span><span class="sxs-lookup"><span data-stu-id="969bc-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="969bc-105">Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.</span><span class="sxs-lookup"><span data-stu-id="969bc-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="969bc-106">Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan.</span><span class="sxs-lookup"><span data-stu-id="969bc-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="969bc-107">Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina.</span><span class="sxs-lookup"><span data-stu-id="969bc-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="969bc-108">Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.</span><span class="sxs-lookup"><span data-stu-id="969bc-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="969bc-109">**DLP-ongelmat ssns**</span><span class="sxs-lookup"><span data-stu-id="969bc-109">**DLP issues with SSNs**</span></span>

<span data-ttu-id="969bc-110">Onko sinulla ongelmia **dlp(Data Loss Prevention) -toiminnon kanssa,** joka ei toimi **sosiaaliturvatunnuksen (SSN)** sisältävän sisällön kanssa, kun käytät arkaluonteista tietotyyppiä Office 365:ssä?</span><span class="sxs-lookup"><span data-stu-id="969bc-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="969bc-111">Jos näin on, varmista, että sisältö sinetaan tarvittavat tiedot siitä, mitä DLP-käytäntö etsii.</span><span class="sxs-lookup"><span data-stu-id="969bc-111">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="969bc-112">Esimerkiksi SSN-käytännölle, jonka luotettavuustaso on 85 %, arvioidaan seuraavat tiedot, ja ne on tunnistettava, jotta sääntö käynnistyy:</span><span class="sxs-lookup"><span data-stu-id="969bc-112">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="969bc-113">**[Muoto:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 numeroa, jotka voivat olla muotoiltutai muotoilematon kuvio</span><span class="sxs-lookup"><span data-stu-id="969bc-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="969bc-114">**[Mallineule:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Neljä toimintoa etsii ssns neljässä eri malleja:</span><span class="sxs-lookup"><span data-stu-id="969bc-114">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="969bc-115">Func_ssn etsii ssn-nijät, joiden muotoilu on ennen vuoden 2011 vahvaa ja jotka on muotoiltu viivoilla tai välilyönneillä (ddd-dd-dddd OR ddd dd ddddd)</span><span class="sxs-lookup"><span data-stu-id="969bc-115">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="969bc-116">Func_unformatted_ssn löytää ssn-nijät, joiden vahva muotoilu on ennen vuotta 2011 ja joita ei ole muotoiltu yhdeksäksi peräkkäiseksi numeroksi (dddddddd)</span><span class="sxs-lookup"><span data-stu-id="969bc-116">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="969bc-117">Func_randomized_formatted_ssn etsii vuoden 2011 jälkeisiä ssn-naatteja, jotka on muotoiltu viivoilla tai välilyönneillä (ddd-dd-ddd OR ddd dd ddddd)</span><span class="sxs-lookup"><span data-stu-id="969bc-117">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="969bc-118">Func_randomized_unformatted_ssn löytää vuoden 2011 jälkeiset ssnit, joita ei ole muotoiltu yhdeksäksi peräkkäiseksi numeroksi (dddddddd)</span><span class="sxs-lookup"><span data-stu-id="969bc-118">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="969bc-119">**[Tarkistussumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ei, ei ole Checksumia.</span><span class="sxs-lookup"><span data-stu-id="969bc-119">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="969bc-120">**[Määritelmä:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP-käytäntö on 85 %: n varma siitä, että se on havainnut tämäntyyppisiä arkaluonteisia tietoja, jos 300 merkin etäisyydellä:</span><span class="sxs-lookup"><span data-stu-id="969bc-120">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="969bc-121">Toiminto [Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) etsii kaavaa vastaavaa sisältöä.</span><span class="sxs-lookup"><span data-stu-id="969bc-121">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="969bc-122">[Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) avainsana löytyy.</span><span class="sxs-lookup"><span data-stu-id="969bc-122">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="969bc-123">Avainsanoja ovat esimerkiksi *sosiaaliturva, sosiaaliturva#, Soc Sec ,SSN* .</span><span class="sxs-lookup"><span data-stu-id="969bc-123">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="969bc-124">Esimerkiksi seuraava esimerkki käynnistäisi DLP SSN -käytännön: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="969bc-124">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="969bc-125">Lisätietoja siitä, mitä sisällön ssn-nimiselle tunnistettaviksi tarvitaan, on tämän artikkelin seuraavassa osassa: [Mitä arkaluonteiset tietotyypit etsivät ssn-verkkoja](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="969bc-125">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="969bc-126">Toisen sisäisen arkaluonteisen tietotyypin avulla on seuraavassa artikkelissa tietoja siitä, mitä muille tyypeille tarvitaan: [Mitä arkaluonteiset tietotyypit etsivät](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="969bc-126">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  