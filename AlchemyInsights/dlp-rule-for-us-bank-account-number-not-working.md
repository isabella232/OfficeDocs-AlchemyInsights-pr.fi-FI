---
title: DLP-sääntö USA:N pankki tilin numerolle ei toimi
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679293"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="55525-102">DLP-ongelmat USA:N pankki tili numeroissa</span><span class="sxs-lookup"><span data-stu-id="55525-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="55525-103">**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="55525-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="55525-104">**DLP-ongelmat USA:N pankki tili numeroissa**</span><span class="sxs-lookup"><span data-stu-id="55525-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="55525-105">Onko sinulla ongelmia **tietojen menetyksen estämisen (DLP)** kanssa, joka ei toimi **Yhdysvaltojen pankki tilin numeron** sisältävässä sisällössä, kun O365-palvelussa käytetään DLP-arkaluonteista tieto tyyppiä?</span><span class="sxs-lookup"><span data-stu-id="55525-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="55525-106">Jos näin on, varmista, että sisältö sisältää tarvittavat tiedot siitä, mitä DLP-käytäntöä etsitään, kun se on laskettu.</span><span class="sxs-lookup"><span data-stu-id="55525-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="55525-107">Esimerkiksi **Yhdysvaltain pankki tilin numero** -käytännölle, jonka luotettavuus taso on 85%, lasketaan seuraavat tiedot ja ne on havaitava, jotta sääntö käynnistetään:</span><span class="sxs-lookup"><span data-stu-id="55525-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="55525-108">**[Muoto:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17-numerot</span><span class="sxs-lookup"><span data-stu-id="55525-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="55525-109">**[Malli:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 peräkkäistä numeroa.</span><span class="sxs-lookup"><span data-stu-id="55525-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="55525-110">**[Tarkistus summa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ei, tarkistus summaa ei ole</span><span class="sxs-lookup"><span data-stu-id="55525-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="55525-111">**[Määritelmä:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP-käytännöllä on 75% varma, että se havaitsee tämän tyyppisiä tietoja, jos se on 300-merkin lähellä:</span><span class="sxs-lookup"><span data-stu-id="55525-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="55525-112">Säännöllinen lauseke Regex_usa_bank_account_number löytää kaavaa vastaavaa sisältöä.</span><span class="sxs-lookup"><span data-stu-id="55525-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="55525-113">Keyword_usa_Bank_Account avain sana löytyy.</span><span class="sxs-lookup"><span data-stu-id="55525-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="55525-114">Esimerkiksi seuraava esimerkki käynnistäisi **USA:n pankki tilin numero** käytäntöä: tarkistetaan tiliä 78344011</span><span class="sxs-lookup"><span data-stu-id="55525-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="55525-115">Lisä tietoja siitä, mitä tarvitaan **USA:n pankki tilin numeron** havaitsemisesta sisältöä varten, on tämän artikkelin seuraavassa osiossa: [mitä luottamukselliset tieto tyypit näyttävät USA:n pankki tili numerolle](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number) ?</span><span class="sxs-lookup"><span data-stu-id="55525-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="55525-116">Jos käytät erilaista sisäistä arkaluonteista tieto tyyppiä, Katso lisä tietoja muista tieto tyypeistä, jotka ovat tarpeen: [mitä luottamukselliset tieto tyypit](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) etsivät</span><span class="sxs-lookup"><span data-stu-id="55525-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  