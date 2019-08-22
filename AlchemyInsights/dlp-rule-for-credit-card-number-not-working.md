---
title: DLP-sääntö, luottokorttinumero ei toimi
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
ms.openlocfilehash: 875afb47175a78c22894720cb0db8222f6f41614
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529952"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="7d094-102">DLP-ongelmia luottokorttinumeroita</span><span class="sxs-lookup"><span data-stu-id="7d094-102">DLP issues with Credit Card Numbers</span></span>

<span data-ttu-id="7d094-103">Onko sinulla ongelmia kanssa **Tietojen menetyksen ehkäisyyn (DLP)** , jossa **Luottokortin numeroa** käytettäessä DLP luottamuksellisten tietojen tyyppi O365 sisällölle ei toimi?</span><span class="sxs-lookup"><span data-stu-id="7d094-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="7d094-104">Jos näin on, varmista, että sisältösi on antamaan tarvittavia tietoja DLP-käytäntö, kun sitä arvioidaan.</span><span class="sxs-lookup"><span data-stu-id="7d094-104">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="7d094-105">Esimerkiksi **luottokortin käytäntö** määritetty 85 %: n varmuudella, seuraavat arvioidaan ja havaittu käynnistää säännön:</span><span class="sxs-lookup"><span data-stu-id="7d094-105">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="7d094-106">**[Muoto:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 numeroa, joka on muotoiltu tai Muotoilematon (dddddddddddddddd) ja on läpäistävä testi Luhn.</span><span class="sxs-lookup"><span data-stu-id="7d094-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="7d094-107">**[Kuvio:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Erittäin monimutkaisia ja vakaan kuvio, joka havaitsee kaikki suuret tuotemerkkejä kaikkialla maailmassa, kuten Visa, MasterCard, löytää kortin, JCB, American Express, lahjakortit, ja kortit diner-kortit.</span><span class="sxs-lookup"><span data-stu-id="7d094-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="7d094-108">**[Tarkistussumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Kyllä, Luhn tarkistussumma</span><span class="sxs-lookup"><span data-stu-id="7d094-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="7d094-109">**[Määritelmä:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP-käytäntö on 85 % varma siitä, että se on havainnut arkaluonteisia henkilötietoja Jos läheisyydessä 300 merkkiä sisällä:</span><span class="sxs-lookup"><span data-stu-id="7d094-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="7d094-110">Func_credit_card-funktio etsii mallia vastaavia kohtia.</span><span class="sxs-lookup"><span data-stu-id="7d094-110">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="7d094-111">Jokin seuraavista pitää paikkansa:</span><span class="sxs-lookup"><span data-stu-id="7d094-111">One of the following is true:</span></span>

  - <span data-ttu-id="7d094-112">-Keyword_cc_verification avainsana on löytynyt.</span><span class="sxs-lookup"><span data-stu-id="7d094-112">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="7d094-113">Avainsana-Keyword_cc_name löytyy</span><span class="sxs-lookup"><span data-stu-id="7d094-113">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="7d094-114">Func_expiration_date-funktio etsii päivämäärä oikean päivämäärän muodossa.</span><span class="sxs-lookup"><span data-stu-id="7d094-114">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="7d094-115">Tarkistussumma osumia</span><span class="sxs-lookup"><span data-stu-id="7d094-115">The checksum passes</span></span>

    <span data-ttu-id="7d094-116">Esimerkiksi seuraava esimerkki aiheuttaa käytännön DLP luottokortin numero:</span><span class="sxs-lookup"><span data-stu-id="7d094-116">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="7d094-117">Viisumi: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="7d094-117">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="7d094-118">Voimassaoloaika päättyy: 2/2009</span><span class="sxs-lookup"><span data-stu-id="7d094-118">Expires: 2/2009</span></span>

<span data-ttu-id="7d094-119">Lisätietoja mitä tarvitaan, jotta voidaan havaita sisällön **Luottokorttinumero** , katso tämän artikkelin seuraavassa osassa: [Mitä on herkkä tietotyypit etsii luottokortin #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="7d094-119">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="7d094-120">Käyttämällä erilaisia sisäisiä luottamuksellisia tietoja, seuraavasta artikkelista lisätietoja, mitä tarvitaan muissa yhteyksissä: [Etsi mitä luottamuksellisten tietojen tyypit](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="7d094-120">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  