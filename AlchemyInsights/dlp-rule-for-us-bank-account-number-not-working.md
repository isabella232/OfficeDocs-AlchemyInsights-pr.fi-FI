---
title: DLP-sääntö, Meille pankkitilinumero ei toimi
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
ms.openlocfilehash: 0a32708b5ac8d95ec6777ada2d151a15f90d65bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529861"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="6e235-102">US pankkitilin numeroita DLP-ongelmia</span><span class="sxs-lookup"><span data-stu-id="6e235-102">DLP issues with US Bank Account Numbers</span></span>

<span data-ttu-id="6e235-103">Onko sinulla ongelmia **Tietojen menetyksen ehkäisyyn (DLP)** ei toimi sisällölle, joka sisältää **US pankkitilinumero** käytettäessä DLP luottamuksellisten tietojen tyypin O365 kanssa?</span><span class="sxs-lookup"><span data-stu-id="6e235-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="6e235-104">Jos näin on, varmista, että sisältö on mitä DLP käytännön etsii kun sen arvioidaan tarvittavat tiedot.</span><span class="sxs-lookup"><span data-stu-id="6e235-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="6e235-105">Esimerkiksi **Yhdysvaltalaisen pankkitilinumero** 85 %: n varmuudella määrittää käytännön, seuraavat arvioidaan ja havaittu käynnistää säännön:</span><span class="sxs-lookup"><span data-stu-id="6e235-105">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="6e235-106">**[Muodossa:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 numeroa</span><span class="sxs-lookup"><span data-stu-id="6e235-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="6e235-107">**[Kuvio:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 peräkkäistä numeroa.</span><span class="sxs-lookup"><span data-stu-id="6e235-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="6e235-108">**[Tarkistussumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ei, ei ole tarkistussumma</span><span class="sxs-lookup"><span data-stu-id="6e235-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="6e235-109">**[Määritelmä:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP-käytäntö on 75 % varma siitä, että se on havainnut arkaluonteisia henkilötietoja Jos läheisyydessä 300 merkkiä sisällä:</span><span class="sxs-lookup"><span data-stu-id="6e235-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="6e235-110">Regex_usa_bank_account_number säännöllinen lauseke löytää sisältöä, joka vastaa kaavaa</span><span class="sxs-lookup"><span data-stu-id="6e235-110">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="6e235-111">-Keyword_usa_Bank_Account avainsana on löytynyt.</span><span class="sxs-lookup"><span data-stu-id="6e235-111">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="6e235-112">Esimerkiksi seuraava esimerkki käynnistää **Yhdysvaltojen pankkitilinumero** käytännön: Sekkitili 78344011</span><span class="sxs-lookup"><span data-stu-id="6e235-112">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="6e235-113">Lisätietoja mitä tarvitaan, jotta voidaan havaita sisällön **Yhdysvaltojen pankkitilinumero** , katso tämän artikkelin seuraavassa osassa: [Mitä on herkkä tietotyypit etsiä US pankkitilinumero](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="6e235-113">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="6e235-114">Käyttämällä erilaisia sisäisiä luottamuksellisia tietoja, seuraavasta artikkelista lisätietoja, mitä tarvitaan muissa yhteyksissä: [Etsi mitä luottamuksellisten tietojen tyypit](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="6e235-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  