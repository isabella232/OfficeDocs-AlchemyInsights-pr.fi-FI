---
title: DLP saattaa tarvita mukautetun tyypin
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712181"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="f5c8d-102">DLP saattaa tarvita mukautetun tyypin</span><span class="sxs-lookup"><span data-stu-id="f5c8d-102">DLP might need a custom type</span></span>

<span data-ttu-id="f5c8d-103">**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="f5c8d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="f5c8d-104">**DLP saattaa edellyttää mukautettua tieto tyyppiä**</span><span class="sxs-lookup"><span data-stu-id="f5c8d-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="f5c8d-105">Tietojen menetyksen estämisen (DLP) käytäntöjen avulla voit tunnistaa ja suojata organisaatiosi luottamukselliset tiedot.</span><span class="sxs-lookup"><span data-stu-id="f5c8d-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="f5c8d-106">Joissakin tilanteissa sinun on ehkä luotava oma **Mukautettu** luottamukselliset tiedot-tyyppi, jotta voit suojata organisaatiosi tiedot.</span><span class="sxs-lookup"><span data-stu-id="f5c8d-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="f5c8d-107">Organisaation on ehkä tunnistettava ja suojattava esimerkiksi työntekijä tunnukset tai muut tiedot jossain tietyssä organisaatiossa. Katso lisä tietoja seuraavista artikkeleista.</span><span class="sxs-lookup"><span data-stu-id="f5c8d-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="f5c8d-108">**Sisäisen arkaluonteisen tieto tyypin mukauttaminen**</span><span class="sxs-lookup"><span data-stu-id="f5c8d-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="f5c8d-109">Jos sisäinen arkaluonteiset tieto tyypit vastaavat tarpeitasi vain muutamalla hienosäädön avulla, voit [mukauttaa valmista arkaluonteista tieto tyyppiä](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="f5c8d-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="f5c8d-110">Voit esimerkiksi lisätä tai poistaa avain sanoja tai lisätä tai poistaa niitä tukevia todisteita, kuten päivä määrän tai osoitteen.</span><span class="sxs-lookup"><span data-stu-id="f5c8d-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="f5c8d-111">**Mukautetun luottamuksellisen tieto tyypin luominen**</span><span class="sxs-lookup"><span data-stu-id="f5c8d-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="f5c8d-112">Jos sinun on tunnistettava ja suojattava erityyppiset luottamukselliset tiedot kokonaan, voit [luoda mukautetun arkaluonteisen tieto tyypin](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) tieto turva & yhteensopivuus keskuksen käyttö liittymässä.</span><span class="sxs-lookup"><span data-stu-id="f5c8d-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="f5c8d-113">**Mukautetun luottamuksellisen tieto tyypin luominen tieto turva & yhteensopivuus keskus PowerShellin avulla**</span><span class="sxs-lookup"><span data-stu-id="f5c8d-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="f5c8d-114">Jos käyttö liittymässä ei ole kaikkia tarvitsemasi vaihto ehtoja, voit [luoda mukautetun arkaluonteisen tieto tyypin tieto turva & yhteensopivuus keskus PowerShellin](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)avulla.</span><span class="sxs-lookup"><span data-stu-id="f5c8d-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="f5c8d-115">Kun aloitat XML-tiedoston avulla, voit käyttää kaikkia käytettävissä olevia vaihto ehtoja.</span><span class="sxs-lookup"><span data-stu-id="f5c8d-115">By starting with an XML file, you can use every option available.</span></span>
