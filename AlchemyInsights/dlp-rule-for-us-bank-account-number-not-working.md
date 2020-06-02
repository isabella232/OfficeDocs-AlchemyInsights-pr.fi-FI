---
title: DLP-sääntö, joka ei toimi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507331"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="4b208-102">DLP-ongelmat Yhdysvaltain pankkitilien numeroiden kanssa</span><span class="sxs-lookup"><span data-stu-id="4b208-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="4b208-103">**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="4b208-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="4b208-104">**DLP-ongelmat Yhdysvaltain pankkitilien numeroiden kanssa**</span><span class="sxs-lookup"><span data-stu-id="4b208-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="4b208-105">Onko sinulla ongelmia, kun tietoja voidaan **ehkäistä DLP (Data Loss Prevention) -toiminnossa,** joka ei toimi sisällössä, joka sisältää **Yhdysvaltain pankkitilin numeron,** käytettäessä DLP-arkaluonteista tietotyyppiä O365:ssä?</span><span class="sxs-lookup"><span data-stu-id="4b208-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="4b208-106">Jos näin on, varmista, että sisältö sisältää tarvittavat tiedot siitä, mitä DLP-käytäntö etsii, kun sitä arvioidaan.</span><span class="sxs-lookup"><span data-stu-id="4b208-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="4b208-107">Esimerkiksi Yhdysvaltain **pankkitilinumerokäytännössä,** jonka luotettavuustaso on 85 %, arvioidaan seuraavat tiedot ja ne on tunnistettava, jotta sääntö käynnistyisi:</span><span class="sxs-lookup"><span data-stu-id="4b208-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="4b208-108">**[Formaatti:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 numeroa</span><span class="sxs-lookup"><span data-stu-id="4b208-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="4b208-109">**[Mallineule:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 peräkkäistä numeroa.</span><span class="sxs-lookup"><span data-stu-id="4b208-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="4b208-110">**[Tarkistussumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ei, tarkistussummaa ei ole.</span><span class="sxs-lookup"><span data-stu-id="4b208-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="4b208-111">**[Määritelmä:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP-käytäntö on 75% varma siitä, että se on havainnut tällaisia arkaluonteisia tietoja, jos 300 merkin läheisyydessä:</span><span class="sxs-lookup"><span data-stu-id="4b208-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="4b208-112">Säännöllinen lauseke Regex_usa_bank_account_number etsii kuviota vastaavaa sisältöä</span><span class="sxs-lookup"><span data-stu-id="4b208-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="4b208-113">Avainsana Keyword_usa_Bank_Account löytyy.</span><span class="sxs-lookup"><span data-stu-id="4b208-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="4b208-114">Esimerkiksi seuraava esimerkki käynnistäisi **Yhdysvaltain** pankkitilinumerokäytännön: Tilin 78344011 tarkistaminen</span><span class="sxs-lookup"><span data-stu-id="4b208-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="4b208-115">Lisätietoja siitä, mitä tarvitaan, jotta **yhdysvaltalainen pankkitilinumero** voidaan havaita sisällöllesi, on tämän artikkelin seuraavassa osassa: [Mitä arkaluonteiset tietotyypit etsivät Yhdysvaltain pankkitilin numeroa](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="4b208-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="4b208-116">Jos käytät eri sisäänrakennettua arkaluonteista tietotyyppiä, lue seuraavassa artikkelissa tietoja siitä, mitä tarvitaan muuntyyppisille [tyypeille: Mitä arkaluonteiset tietotyypit etsivät](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="4b208-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  