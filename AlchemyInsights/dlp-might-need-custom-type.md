---
title: DLP saattaa tarvita mukautetun tyypin
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 872fca326065ada002300061c951620b3d9a8d0e
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052898"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="018ab-102">DLP saattaa tarvita mukautetun tyypin</span><span class="sxs-lookup"><span data-stu-id="018ab-102">DLP might need a custom type</span></span>

<span data-ttu-id="018ab-103">Tietojen menetyksen eston (DLP) käytännön avulla voit tunnistaa ja suojata organisaatiosi luottamukselliset tiedot.</span><span class="sxs-lookup"><span data-stu-id="018ab-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="018ab-104">Joissakin tilanteissa sinun on ehkä luotava oma **Mukautettu** arkaluonteinen tieto tyyppi organisaatiosi tietojen suojaamiseksi.</span><span class="sxs-lookup"><span data-stu-id="018ab-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="018ab-105">Organisaatiosi on ehkä esimerkiksi tunnistettava ja suojattava työntekijä tunnukset tai muut tiedot tietyssä organisaatiosi muodossa. Jos näin on, Katso lisä tietoja seuraavista artikkeleista.</span><span class="sxs-lookup"><span data-stu-id="018ab-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="018ab-106">**Sisäisen arkaluonteisen tieto tyypin mukauttaminen**</span><span class="sxs-lookup"><span data-stu-id="018ab-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="018ab-107">Jos sisäinen arkaluonteinen tieto tyyppi vastaa tarpeitasi vain muutamalla hienosäällä, voit [mukauttaa sisäistä arkaluontoista tieto tyyppiä](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="018ab-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="018ab-108">Voit esimerkiksi lisätä tai poistaa avain sanoja tai lisätä tai poistaa tuki todisteita, kuten päivä määrän tai osoitteen.</span><span class="sxs-lookup"><span data-stu-id="018ab-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="018ab-109">**Mukautetun arkaluonteisen tieto tyypin luominen**</span><span class="sxs-lookup"><span data-stu-id="018ab-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="018ab-110">Mutta jos sinun on tunnistettava ja suojattava erityyppisiä arkaluonteisia tietoja kokonaan, voit [luoda mukautetun arkaluonteisen tieto tyypin](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) suojaus & yhteensopivuus keskuksen käyttö liittymässä.</span><span class="sxs-lookup"><span data-stu-id="018ab-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="018ab-111">**Mukautetun arkaluonteisen tieto tyypin luominen suojaus & yhteensopivuus keskuksessa PowerShell**</span><span class="sxs-lookup"><span data-stu-id="018ab-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="018ab-112">Lopuksi, jos käyttö liittymä ei tarjoa kaikkia tarvitsemiansa vaihto ehtoja, voit [luoda mukautetun luottamukselliset tiedot-tyypin Security & Compliance Center PowerShellin](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="018ab-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="018ab-113">Kun aloitat XML-tiedostosta, voit käyttää jokaista käytettävissä olevaa vaihto ehtoa.</span><span class="sxs-lookup"><span data-stu-id="018ab-113">By starting with an XML file, you can use every option available.</span></span>
