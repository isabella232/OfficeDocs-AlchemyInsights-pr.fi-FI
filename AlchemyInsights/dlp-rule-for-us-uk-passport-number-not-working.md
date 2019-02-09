---
title: DLP-säännön USA / UK passin numero ei toimi
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: ec7f11676982b56a46c83bf276c2212ce765ba6f
ms.sourcegitcommit: ca06ef831226d629de3057a0df85e017b80f3356
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/08/2019
ms.locfileid: "29786695"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="0328f-102">DLP - ongelmia US / UK passi numerot</span><span class="sxs-lookup"><span data-stu-id="0328f-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="0328f-p101">Onko sinulla ongelmia **Tietojen menetyksen ehkäisyyn (DLP)** ei toimi, joka sisältää sisällön kanssa **USA / UK passin numero** käytettäessä DLP luottamuksellisten tietojen tyyppi O365? Jos näin on, varmista, että sisältö on mitä DLP käytännön etsii kun sen arvioidaan tarvittavat tiedot.</span><span class="sxs-lookup"><span data-stu-id="0328f-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="0328f-105">Esimerkiksi **USA / UK passin numero** 75 %: n varmuudella määritetty käytäntö, seuraavat arvioidaan ja käynnistää sääntö on havaittavissa</span><span class="sxs-lookup"><span data-stu-id="0328f-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="0328f-106">**[Muodossa:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Yhdeksän numeroa</span><span class="sxs-lookup"><span data-stu-id="0328f-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="0328f-107">**[Kuvio:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Yhdeksän peräkkäistä numeroa</span><span class="sxs-lookup"><span data-stu-id="0328f-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="0328f-108">**[Tarkistussumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ei, ei ole tarkistussumma</span><span class="sxs-lookup"><span data-stu-id="0328f-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="0328f-109">**[Määritelmä:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP-käytäntö on 75 % varma siitä, että se on havainnut arkaluonteisia henkilötietoja Jos läheisyydessä 300 merkkiä sisällä:</span><span class="sxs-lookup"><span data-stu-id="0328f-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="0328f-110">Func_usa_uk_passport-funktio etsii mallia vastaavia kohtia.</span><span class="sxs-lookup"><span data-stu-id="0328f-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="0328f-111">-Keyword_passport avainsana on löytynyt.</span><span class="sxs-lookup"><span data-stu-id="0328f-111">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="0328f-112">Esimerkiksi seuraava malli käynnistää **USA / UK passin numero** käytännön: Yhdysvaltain passin numero 123456789</span><span class="sxs-lookup"><span data-stu-id="0328f-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="0328f-113">Lisätietoja mitä tarvitaan USA / UK passin numero, sisällön tunnistaminen on tämän artikkelin seuraavassa osassa: [Etsi mitä luottamuksellisten tietojen tyypit USA / UK passin numero](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="0328f-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="0328f-114">Käyttämällä erilaisia sisäisiä luottamuksellisia tietoja, seuraavasta artikkelista lisätietoja, mitä tarvitaan muissa yhteyksissä: [Etsi mitä luottamuksellisten tietojen tyypit](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="0328f-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

