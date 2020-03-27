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
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977103"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="7c9b0-102">Ongelmia DLP - USA / Iso-Britannia passin numerot</span><span class="sxs-lookup"><span data-stu-id="7c9b0-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="7c9b0-103">**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat edelleen erittäin saatavilla – lisätietoja on [SharePoint Onlinen tilapäisissä ominaisuusoikaisuissa.](https://aka.ms/ODSPAdjustments)</span><span class="sxs-lookup"><span data-stu-id="7c9b0-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="7c9b0-104">**DLP-ongelmat Yhdysvaltain ja Yhdistyneen kuningaskunnan passinumeroiden kanssa**</span><span class="sxs-lookup"><span data-stu-id="7c9b0-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="7c9b0-105">Onko sinulla ongelmia **Data Loss Prevention (DLP)** ei toimi sisältöä, joka sisältää Yhdysvaltain ja Yhdistyneen **kuningaskunnan passin numero,** kun käytät DLP arkaluonteisia tietoja tyyppi O365?</span><span class="sxs-lookup"><span data-stu-id="7c9b0-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="7c9b0-106">Jos näin on, varmista, että sisältösi sisältää tarvittavat tiedot siitä, mitä DLP-käytäntö etsii, kun sitä arvioidaan.</span><span class="sxs-lookup"><span data-stu-id="7c9b0-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="7c9b0-107">Esimerkiksi Yhdysvaltain **ja Yhdistyneen kuningaskunnan passin numerokäytännössä,** jonka luotettavuustaso on 75 %, arvioidaan seuraavat tiedot, ja ne on tunnistettava, jotta sääntö voi käynnistää</span><span class="sxs-lookup"><span data-stu-id="7c9b0-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="7c9b0-108">**[Muoto:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Yhdeksän numeroa</span><span class="sxs-lookup"><span data-stu-id="7c9b0-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="7c9b0-109">**[Mallineule:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Yhdeksän peräkkäistä numeroa</span><span class="sxs-lookup"><span data-stu-id="7c9b0-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="7c9b0-110">**[Tarkistussumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ei, ei ole Checksumia.</span><span class="sxs-lookup"><span data-stu-id="7c9b0-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="7c9b0-111">**[Määritelmä:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP-käytäntö on 75 %: n varma siitä, että se on havainnut tämäntyyppisiä arkaluonteisia tietoja, jos 300 merkin etäisyydellä:</span><span class="sxs-lookup"><span data-stu-id="7c9b0-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="7c9b0-112">Toiminto Func_usa_uk_passport etsii kaavaa vastaavaa sisältöä.</span><span class="sxs-lookup"><span data-stu-id="7c9b0-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="7c9b0-113">Keyword_passport avainsana löytyy.</span><span class="sxs-lookup"><span data-stu-id="7c9b0-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="7c9b0-114">Esimerkiksi seuraava esimerkki käynnistäisi **Yhdysvaltain ja Yhdistyneen kuningaskunnan passinumerokäytännön:** Yhdysvaltain passin numero 123456789</span><span class="sxs-lookup"><span data-stu-id="7c9b0-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="7c9b0-115">Lisätietoja siitä, mitä tarvitaan, jotta Yhdysvaltain ja Yhdistyneen kuningaskunnan passinumero voidaan havaita sisällöllesi, on tämän artikkelin seuraavassa osassa: [Mitä arkaluonteiset tietotyypit etsivät YHDYSVALTAIN ja Yhdistyneen kuningaskunnan passin numeroa](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="7c9b0-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="7c9b0-116">Toisen sisäisen arkaluonteisen tietotyypin avulla on seuraavassa artikkelissa tietoja siitä, mitä muille tyypeille tarvitaan: [Mitä arkaluonteiset tietotyypit etsivät](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="7c9b0-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  