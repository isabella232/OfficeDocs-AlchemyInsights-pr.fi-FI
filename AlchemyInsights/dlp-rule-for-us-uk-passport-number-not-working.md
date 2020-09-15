---
title: DLP-sääntö YHDYSVALTALLE/UK:N Passport-numerolle ei toimi
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679221"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="720f3-102">DLP-US/UK Passport-numeroiden ongelmat</span><span class="sxs-lookup"><span data-stu-id="720f3-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="720f3-103">**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="720f3-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="720f3-104">**DLP-ongelmat USA:N/Yhdistyneen kuningas kunnan Passport-numeroissa**</span><span class="sxs-lookup"><span data-stu-id="720f3-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="720f3-105">Onko sinulla ongelmia **tietojen menetyksen estämisen (DLP)** kanssa, joka ei toimi **Yhdysvalloissa ja Yhdistyneessä kuningas kunnassa olevan Passport-numeron** sisältävässä sisällössä, kun O365-palvelussa käytetään DLP-arkaluonteista tieto tyyppiä?</span><span class="sxs-lookup"><span data-stu-id="720f3-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="720f3-106">Jos näin on, varmista, että sisältö sisältää tarvittavat tiedot siitä, mitä DLP-käytäntöä etsitään, kun se on laskettu.</span><span class="sxs-lookup"><span data-stu-id="720f3-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="720f3-107">Esimerkiksi **Yhdysvaltain ja Yhdistyneen kuningas kunnan passin numero** käytännölle, jonka luotettavuus taso on 75%, lasketaan seuraavat ehdot, jotka on määritettävä, jotta sääntö käynnistetään</span><span class="sxs-lookup"><span data-stu-id="720f3-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="720f3-108">**[Muoto:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Yhdeksän numeroa</span><span class="sxs-lookup"><span data-stu-id="720f3-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="720f3-109">**[Malli neule:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Yhdeksän peräkkäistä numeroa</span><span class="sxs-lookup"><span data-stu-id="720f3-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="720f3-110">**[Tarkistus summa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ei, tarkistus summaa ei ole</span><span class="sxs-lookup"><span data-stu-id="720f3-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="720f3-111">**[Määritelmä:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP-käytännöllä on 75% varma, että se havaitsee tämän tyyppisiä tietoja, jos se on 300-merkin lähellä:</span><span class="sxs-lookup"><span data-stu-id="720f3-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="720f3-112">Funktio Func_usa_uk_passport löytää kaavaa vastaavaa sisältöä.</span><span class="sxs-lookup"><span data-stu-id="720f3-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="720f3-113">Keyword_passport avain sana löytyy.</span><span class="sxs-lookup"><span data-stu-id="720f3-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="720f3-114">Esimerkiksi seuraava esimerkki käynnistäisi **Yhdysvaltojen ja Yhdistyneen kuningas kunnan passin numero** käytäntöä: Yhdysvaltain passin numero 123456789</span><span class="sxs-lookup"><span data-stu-id="720f3-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="720f3-115">Lisä tietoja käyttäjän ja Yhdistyneen kuningas kunnan passin numeron havaitsemisesta sisältöä varten on tämän artikkelin seuraavassa osiossa: [mitä luottamukselliset tieto tyypit näyttävät Yhdysvaltojen ja Yhdistyneen kuningas kunnan Passport-numerolle](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="720f3-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="720f3-116">Jos käytät erilaista sisäistä arkaluonteista tieto tyyppiä, Katso lisä tietoja muista tieto tyypeistä, jotka ovat tarpeen: [mitä luottamukselliset tieto tyypit](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) etsivät</span><span class="sxs-lookup"><span data-stu-id="720f3-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  