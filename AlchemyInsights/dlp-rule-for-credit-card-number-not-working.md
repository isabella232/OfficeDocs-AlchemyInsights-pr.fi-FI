---
title: Luottokortin numeron DLP-sääntö ei toimi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932440"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="2f70a-102">DLP-ongelmat luottokorttien numeroissa</span><span class="sxs-lookup"><span data-stu-id="2f70a-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="2f70a-103">**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan.</span><span class="sxs-lookup"><span data-stu-id="2f70a-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="2f70a-104">Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut.</span><span class="sxs-lookup"><span data-stu-id="2f70a-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="2f70a-105">Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.</span><span class="sxs-lookup"><span data-stu-id="2f70a-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="2f70a-106">Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan.</span><span class="sxs-lookup"><span data-stu-id="2f70a-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="2f70a-107">Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina.</span><span class="sxs-lookup"><span data-stu-id="2f70a-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="2f70a-108">Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.</span><span class="sxs-lookup"><span data-stu-id="2f70a-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="2f70a-109">**DLP-ongelmat luottokorttien numeroissa**</span><span class="sxs-lookup"><span data-stu-id="2f70a-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="2f70a-110">Onko sinulla ongelmia **DLP (Data Loss Prevention) -toiminnon kanssa,** joka ei toimi **luottokortin numeron** sisältävän sisällön kanssa, kun käytät DLP-arkaluonteista tietotyyppiä O365:ssä?</span><span class="sxs-lookup"><span data-stu-id="2f70a-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="2f70a-111">Jos näin on, varmista, että sisältösi sisältää tarvittavat tiedot DLP-käytännön käynnistämiseen, kun sitä arvioidaan.</span><span class="sxs-lookup"><span data-stu-id="2f70a-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="2f70a-112">Esimerkiksi **luottokorttikäytännössä,** jonka luotettavuustaso on 85 %, arvioidaan seuraavat tiedot, ja ne on tunnistettava, jotta sääntö käynnistyy:</span><span class="sxs-lookup"><span data-stu-id="2f70a-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="2f70a-113">**[Muoto:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 numeroa, jotka voidaan muotoilla tai muotoilematon (ddddddddddddddddddddddddddddddd.</span><span class="sxs-lookup"><span data-stu-id="2f70a-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="2f70a-114">**[Mallineule:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Erittäin monimutkainen ja vankka kuvio, joka havaitsee kortit kaikilta maailman suurilta brändeiltä, mukaan lukien Visa, MasterCard, Discover Card, JCB, American Express, lahjakortit ja diner-kortit.</span><span class="sxs-lookup"><span data-stu-id="2f70a-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="2f70a-115">**[Tarkistussumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Kyllä, Luhnin tarkistussumma</span><span class="sxs-lookup"><span data-stu-id="2f70a-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="2f70a-116">**[Määritelmä:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP-käytäntö on 85 %: n varma siitä, että se on havainnut tämäntyyppisiä arkaluonteisia tietoja, jos 300 merkin etäisyydellä:</span><span class="sxs-lookup"><span data-stu-id="2f70a-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="2f70a-117">Funktio Func_credit_card etsii kaavaa vastaavaa sisältöä.</span><span class="sxs-lookup"><span data-stu-id="2f70a-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="2f70a-118">Jokin seuraavista on totta:</span><span class="sxs-lookup"><span data-stu-id="2f70a-118">One of the following is true:</span></span>

  - <span data-ttu-id="2f70a-119">Keyword_cc_verification avainsana löytyy.</span><span class="sxs-lookup"><span data-stu-id="2f70a-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="2f70a-120">Keyword_cc_name avainsana löytyy</span><span class="sxs-lookup"><span data-stu-id="2f70a-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="2f70a-121">Funktio Func_expiration_date löytää päivämäärän oikeassa päivämäärämuodossa.</span><span class="sxs-lookup"><span data-stu-id="2f70a-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="2f70a-122">Tarkistussumma kulkee</span><span class="sxs-lookup"><span data-stu-id="2f70a-122">The checksum passes</span></span>

    <span data-ttu-id="2f70a-123">Esimerkiksi seuraava esimerkki käynnistidänsä DLP-luottokortin numerokäytännön:</span><span class="sxs-lookup"><span data-stu-id="2f70a-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="2f70a-124">Viisumi: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="2f70a-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="2f70a-125">Päättyy: 2/2009</span><span class="sxs-lookup"><span data-stu-id="2f70a-125">Expires: 2/2009</span></span>

<span data-ttu-id="2f70a-126">Lisätietoja siitä, mitä vaaditaan, jotta **luottokorttinumero** voidaan havaita sisällöllesi, on tämän artikkelin seuraavassa osassa: [Mitä arkaluonteiset tietotyypit etsivät luottokorttia#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="2f70a-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="2f70a-127">Toisen sisäisen arkaluonteisen tietotyypin avulla on seuraavassa artikkelissa tietoja siitä, mitä muille tyypeille tarvitaan: [Mitä arkaluonteiset tietotyypit etsivät](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="2f70a-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  