---
title: DLP-sääntö luottokortin numerolle ei toimi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507403"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="c33e0-102">DLP-ongelmat luottokorttien numeroiden kanssa</span><span class="sxs-lookup"><span data-stu-id="c33e0-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="c33e0-103">**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="c33e0-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="c33e0-104">**DLP-ongelmat luottokorttien numeroiden kanssa**</span><span class="sxs-lookup"><span data-stu-id="c33e0-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="c33e0-105">Onko sinulla ongelmia **tietojen menetyksen estämisessä (DLP)** ei toimi sisällössä, joka sisältää **luottokortin numeron,** kun käytät DLP-arkaluonteista tietotyyppiä O365:ssä?</span><span class="sxs-lookup"><span data-stu-id="c33e0-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="c33e0-106">Jos näin on, varmista, että sisältö sisältää tarvittavat tiedot, jotta DLP-käytäntö käynnistetään, kun sitä arvioidaan.</span><span class="sxs-lookup"><span data-stu-id="c33e0-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="c33e0-107">Esimerkiksi **luottokorttikäytännössä,** jonka luotettavuustaso on 85 %, arvioidaan seuraavat tiedot, jotka on tunnistettava, jotta sääntö käynnistyisi:</span><span class="sxs-lookup"><span data-stu-id="c33e0-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="c33e0-108">**[Muoto:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 numeroa, jotka voidaan muotoilla tai alustamatta (dddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd</span><span class="sxs-lookup"><span data-stu-id="c33e0-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="c33e0-109">**[Mallineule:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Erittäin monimutkainen ja vankka kuvio, joka havaitsee kortteja kaikista tärkeimmistä tuotemerkeistä maailmanlaajuisesti, mukaan lukien Visa, MasterCard, Discover Card, JCB, American Express, lahjakortit ja diner-kortit.</span><span class="sxs-lookup"><span data-stu-id="c33e0-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="c33e0-110">**[Tarkistussumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Kyllä, Luhnin tarkistussumma.</span><span class="sxs-lookup"><span data-stu-id="c33e0-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="c33e0-111">**[Määritelmä:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP-käytäntö on 85% varma siitä, että se on havainnut tällaisia arkaluonteisia tietoja, jos 300 merkin läheisyydessä:</span><span class="sxs-lookup"><span data-stu-id="c33e0-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="c33e0-112">Funktio, Func_credit_card etsii kuviota vastaavaa sisältöä.</span><span class="sxs-lookup"><span data-stu-id="c33e0-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="c33e0-113">Jokin seuraavista on totta:</span><span class="sxs-lookup"><span data-stu-id="c33e0-113">One of the following is true:</span></span>

  - <span data-ttu-id="c33e0-114">Avainsana Keyword_cc_verification löytyy.</span><span class="sxs-lookup"><span data-stu-id="c33e0-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="c33e0-115">Avainsana Keyword_cc_name löytyy</span><span class="sxs-lookup"><span data-stu-id="c33e0-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="c33e0-116">Funktio, Func_expiration_date etsii päivämäärän oikeassa päivämäärämuodossa.</span><span class="sxs-lookup"><span data-stu-id="c33e0-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="c33e0-117">Tarkistussumma kulkee</span><span class="sxs-lookup"><span data-stu-id="c33e0-117">The checksum passes</span></span>

    <span data-ttu-id="c33e0-118">Esimerkiksi seuraava esimerkki käynnistäisi DLP-luottokortin numerokäytännön:</span><span class="sxs-lookup"><span data-stu-id="c33e0-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="c33e0-119">Viisumi: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="c33e0-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="c33e0-120">Päättyy: 2/2009</span><span class="sxs-lookup"><span data-stu-id="c33e0-120">Expires: 2/2009</span></span>

<span data-ttu-id="c33e0-121">Lisätietoja siitä, mitä tarvitaan, jotta **luottokorttinumero** voidaan havaita sisällöllesi, on tämän artikkelin seuraavassa osassa: [Mitä arkaluonteiset tietotyypit etsivät luottokorttia#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="c33e0-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="c33e0-122">Jos käytät eri sisäänrakennettua arkaluonteista tietotyyppiä, lue seuraavassa artikkelissa tietoja siitä, mitä tarvitaan muuntyyppisille [tyypeille: Mitä arkaluonteiset tietotyypit etsivät](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="c33e0-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  