---
title: DLP sääntö YHDYSVALTAIN / UK Passport Number ei toimi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931259"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="dad1b-102">Ongelmia DLP - USA / Iso-Britannia passin numerot</span><span class="sxs-lookup"><span data-stu-id="dad1b-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="dad1b-103">**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan.</span><span class="sxs-lookup"><span data-stu-id="dad1b-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="dad1b-104">Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut.</span><span class="sxs-lookup"><span data-stu-id="dad1b-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="dad1b-105">Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.</span><span class="sxs-lookup"><span data-stu-id="dad1b-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="dad1b-106">Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan.</span><span class="sxs-lookup"><span data-stu-id="dad1b-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="dad1b-107">Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina.</span><span class="sxs-lookup"><span data-stu-id="dad1b-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="dad1b-108">Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.</span><span class="sxs-lookup"><span data-stu-id="dad1b-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="dad1b-109">**DLP-ongelmat Yhdysvaltain ja Yhdistyneen kuningaskunnan passinumeroiden kanssa**</span><span class="sxs-lookup"><span data-stu-id="dad1b-109">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="dad1b-110">Onko sinulla ongelmia **Data Loss Prevention (DLP)** ei toimi sisältöä, joka sisältää Yhdysvaltain ja Yhdistyneen **kuningaskunnan passin numero,** kun käytät DLP arkaluonteisia tietoja tyyppi O365?</span><span class="sxs-lookup"><span data-stu-id="dad1b-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="dad1b-111">Jos näin on, varmista, että sisältösi sisältää tarvittavat tiedot siitä, mitä DLP-käytäntö etsii, kun sitä arvioidaan.</span><span class="sxs-lookup"><span data-stu-id="dad1b-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="dad1b-112">Esimerkiksi Yhdysvaltain **ja Yhdistyneen kuningaskunnan passin numerokäytännössä,** jonka luotettavuustaso on 75 %, arvioidaan seuraavat tiedot, ja ne on tunnistettava, jotta sääntö voi käynnistää</span><span class="sxs-lookup"><span data-stu-id="dad1b-112">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="dad1b-113">**[Muoto:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Yhdeksän numeroa</span><span class="sxs-lookup"><span data-stu-id="dad1b-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="dad1b-114">**[Mallineule:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Yhdeksän peräkkäistä numeroa</span><span class="sxs-lookup"><span data-stu-id="dad1b-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="dad1b-115">**[Tarkistussumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ei, ei ole Checksumia.</span><span class="sxs-lookup"><span data-stu-id="dad1b-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="dad1b-116">**[Määritelmä:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP-käytäntö on 75 %: n varma siitä, että se on havainnut tämäntyyppisiä arkaluonteisia tietoja, jos 300 merkin etäisyydellä:</span><span class="sxs-lookup"><span data-stu-id="dad1b-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="dad1b-117">Toiminto Func_usa_uk_passport etsii kaavaa vastaavaa sisältöä.</span><span class="sxs-lookup"><span data-stu-id="dad1b-117">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="dad1b-118">Keyword_passport avainsana löytyy.</span><span class="sxs-lookup"><span data-stu-id="dad1b-118">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="dad1b-119">Esimerkiksi seuraava esimerkki käynnistäisi **Yhdysvaltain ja Yhdistyneen kuningaskunnan passinumerokäytännön:** Yhdysvaltain passin numero 123456789</span><span class="sxs-lookup"><span data-stu-id="dad1b-119">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="dad1b-120">Lisätietoja siitä, mitä tarvitaan, jotta Yhdysvaltain ja Yhdistyneen kuningaskunnan passinumero voidaan havaita sisällöllesi, on tämän artikkelin seuraavassa osassa: [Mitä arkaluonteiset tietotyypit etsivät YHDYSVALTAIN ja Yhdistyneen kuningaskunnan passin numeroa](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="dad1b-120">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="dad1b-121">Toisen sisäisen arkaluonteisen tietotyypin avulla on seuraavassa artikkelissa tietoja siitä, mitä muille tyypeille tarvitaan: [Mitä arkaluonteiset tietotyypit etsivät](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="dad1b-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  