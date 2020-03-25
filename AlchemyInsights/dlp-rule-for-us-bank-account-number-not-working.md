---
title: Yhdysvaltain pankkitilin numeron DLP-sääntö ei toimi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932528"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="9e442-102">DLP-ongelmat yhdysvaltalaisissa tilinumeroissa</span><span class="sxs-lookup"><span data-stu-id="9e442-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="9e442-103">**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan.</span><span class="sxs-lookup"><span data-stu-id="9e442-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="9e442-104">Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut.</span><span class="sxs-lookup"><span data-stu-id="9e442-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="9e442-105">Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.</span><span class="sxs-lookup"><span data-stu-id="9e442-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="9e442-106">Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan.</span><span class="sxs-lookup"><span data-stu-id="9e442-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="9e442-107">Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina.</span><span class="sxs-lookup"><span data-stu-id="9e442-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="9e442-108">Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.</span><span class="sxs-lookup"><span data-stu-id="9e442-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="9e442-109">**DLP-ongelmat yhdysvaltalaisissa tilinumeroissa**</span><span class="sxs-lookup"><span data-stu-id="9e442-109">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="9e442-110">Onko sinulla ongelmia **DLP (Data Loss Prevention) -toiminnon kanssa,** joka ei toimi sisällössä, joka sisältää **Yhdysvaltain pankkitilinumeron,** kun käytät DLP-arkaluonteista tietotyyppiä O365:ssä?</span><span class="sxs-lookup"><span data-stu-id="9e442-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="9e442-111">Jos näin on, varmista, että sisältösi sisältää tarvittavat tiedot siitä, mitä DLP-käytäntö etsii, kun sitä arvioidaan.</span><span class="sxs-lookup"><span data-stu-id="9e442-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="9e442-112">Esimerkiksi YHDYSVALTAIN **pankkitilin numero -käytännössä,** jonka luotettavuustaso on 85 %, arvioidaan seuraavat tiedot, ja ne on tunnistettava, jotta sääntö käynnistyy:</span><span class="sxs-lookup"><span data-stu-id="9e442-112">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="9e442-113">**[Formaatti:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 numeroa</span><span class="sxs-lookup"><span data-stu-id="9e442-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="9e442-114">**[Mallineule:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 peräkkäistä numeroa.</span><span class="sxs-lookup"><span data-stu-id="9e442-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="9e442-115">**[Tarkistussumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ei, ei ole Checksumia.</span><span class="sxs-lookup"><span data-stu-id="9e442-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="9e442-116">**[Määritelmä:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP-käytäntö on 75 %: n varma siitä, että se on havainnut tämäntyyppisiä arkaluonteisia tietoja, jos 300 merkin etäisyydellä:</span><span class="sxs-lookup"><span data-stu-id="9e442-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="9e442-117">Säännöllinen lauseke Regex_usa_bank_account_number etsii kaavaa vastaavaa sisältöä</span><span class="sxs-lookup"><span data-stu-id="9e442-117">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="9e442-118">Keyword_usa_Bank_Account avainsana löytyy.</span><span class="sxs-lookup"><span data-stu-id="9e442-118">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="9e442-119">Esimerkiksi seuraava esimerkki **käynnistisi Yhdysvaltain pankkitilin numero -käytännön:** Tilin 78344011 tarkistaminen</span><span class="sxs-lookup"><span data-stu-id="9e442-119">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="9e442-120">Lisätietoja siitä, mitä vaaditaan, jotta **Yhdysvaltalainen pankkitilinumero** voidaan havaita sisällöllesi, on tämän artikkelin seuraavassa osassa: [Mitä arkaluonteiset tietotyypit etsivät Yhdysvaltain pankkitilinumeroa](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="9e442-120">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="9e442-121">Toisen sisäisen arkaluonteisen tietotyypin avulla on seuraavassa artikkelissa tietoja siitä, mitä muille tyypeille tarvitaan: [Mitä arkaluonteiset tietotyypit etsivät](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="9e442-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  