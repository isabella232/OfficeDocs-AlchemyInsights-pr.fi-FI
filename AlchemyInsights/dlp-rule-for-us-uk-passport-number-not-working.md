---
title: US/UK Passport -passin numero ei toimi DLP-sääntö
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507295"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="d0b02-102">Ongelmia DLP - USA / UK passin numerot</span><span class="sxs-lookup"><span data-stu-id="d0b02-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="d0b02-103">**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="d0b02-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d0b02-104">**DLP-ongelmat Yhdysvaltain ja Yhdistyneen kuningaskunnan passinumeroiden kanssa**</span><span class="sxs-lookup"><span data-stu-id="d0b02-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="d0b02-105">Onko sinulla ongelmia, kun **käytät DLP-arkaluonteista** tietotyyppiä O365:ssä, **kun** käytät DLP-arkaluonteista tietotyyppiä O365:ssä?</span><span class="sxs-lookup"><span data-stu-id="d0b02-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="d0b02-106">Jos näin on, varmista, että sisältö sisältää tarvittavat tiedot siitä, mitä DLP-käytäntö etsii, kun sitä arvioidaan.</span><span class="sxs-lookup"><span data-stu-id="d0b02-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="d0b02-107">Esimerkiksi Yhdysvaltain **ja Yhdistyneen kuningaskunnan passinumerokäytännössä,** jonka luotettavuustaso on 75 %, arvioidaan seuraavat tiedot ja ne on tunnistettava, jotta sääntö käynnistää</span><span class="sxs-lookup"><span data-stu-id="d0b02-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="d0b02-108">**[Muoto:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Yhdeksän numeroa</span><span class="sxs-lookup"><span data-stu-id="d0b02-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="d0b02-109">**[Mallineule:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Yhdeksän peräkkäistä numeroa</span><span class="sxs-lookup"><span data-stu-id="d0b02-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="d0b02-110">**[Tarkistussumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ei, tarkistussummaa ei ole.</span><span class="sxs-lookup"><span data-stu-id="d0b02-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="d0b02-111">**[Määritelmä:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP-käytäntö on 75% varma siitä, että se on havainnut tällaisia arkaluonteisia tietoja, jos 300 merkin läheisyydessä:</span><span class="sxs-lookup"><span data-stu-id="d0b02-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d0b02-112">Funktio Func_usa_uk_passport etsii kuviota vastaavaa sisältöä.</span><span class="sxs-lookup"><span data-stu-id="d0b02-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="d0b02-113">Avainsana Keyword_passport löytyy.</span><span class="sxs-lookup"><span data-stu-id="d0b02-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="d0b02-114">Esimerkiksi seuraava esimerkki käynnistäisi **Yhdysvaltain ja Yhdistyneen kuningaskunnan passinumerokäytännön:** Yhdysvaltain passin numero 123456789</span><span class="sxs-lookup"><span data-stu-id="d0b02-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="d0b02-115">Lisätietoja siitä, mitä tarvitaan, jotta Yhdysvaltalaisen ja Yhdistyneen kuningaskunnan passinumero voidaan havaita sisällöllesi, on tämän artikkelin seuraavassa osassa: [Mitä arkaluonteiset tietotyypit etsivät Yhdysvaltain ja Yhdistyneen kuningaskunnan passinumeroa](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="d0b02-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="d0b02-116">Jos käytät eri sisäänrakennettua arkaluonteista tietotyyppiä, lue seuraavassa artikkelissa tietoja siitä, mitä tarvitaan muuntyyppisille [tyypeille: Mitä arkaluonteiset tietotyypit etsivät](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="d0b02-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  