---
title: DLP saattaa tarvita mukautetun tyypin
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507511"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="60fb5-102">DLP saattaa tarvita mukautetun tyypin</span><span class="sxs-lookup"><span data-stu-id="60fb5-102">DLP might need a custom type</span></span>

<span data-ttu-id="60fb5-103">**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="60fb5-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="60fb5-104">**DLP saattaa edellyttää mukautettua tietotyyppiä**</span><span class="sxs-lookup"><span data-stu-id="60fb5-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="60fb5-105">DLP (Data Loss Prevention) -käytännön avulla voit tunnistaa ja suojata organisaation arkaluonteiset tiedot.</span><span class="sxs-lookup"><span data-stu-id="60fb5-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="60fb5-106">Joissakin tilanteissa sinun on ehkä luotava oma **mukautettu** arkaluonteinen tietotyyppi, jotta voit suojata organisaatiosi tiedot.</span><span class="sxs-lookup"><span data-stu-id="60fb5-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="60fb5-107">Organisaatiosi on ehkä esimerkiksi tunnistettava ja suojattava työntekijätunnukset tai muut tiedot organisaatiollesi tietyssä muodossa. Jos näin on, katso lisätietoja seuraavista artikkeleista.</span><span class="sxs-lookup"><span data-stu-id="60fb5-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="60fb5-108">**Valmiin arkaluonteisen tietotyypin mukauttaminen**</span><span class="sxs-lookup"><span data-stu-id="60fb5-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="60fb5-109">Jos sisäänrakennettu arkaluonteinen tietotyyppi vastaisi tarpeitasi muutamalla hienosäädöllä, voit [mukauttaa sisäänrakennettua arkaluonteista tietotyyppiä](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="60fb5-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="60fb5-110">Voit esimerkiksi lisätä tai poistaa avainsanoja tai lisätä tai poistaa todisteita, kuten päivämäärän tai osoitteen.</span><span class="sxs-lookup"><span data-stu-id="60fb5-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="60fb5-111">**Mukautetun arkaluonteisen tietotyypin luominen**</span><span class="sxs-lookup"><span data-stu-id="60fb5-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="60fb5-112">Jos sinun on kuitenkin tunnistettava ja suojattava erityyppiset arkaluonteiset tiedot kokonaan, voit [luoda mukautetun arkaluonteisen tietotyypin](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) Tietoturva-& Compliance Centerin käyttöliittymään.</span><span class="sxs-lookup"><span data-stu-id="60fb5-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="60fb5-113">**Mukautetun arkaluonteisen tietotyypin luominen Security & Compliance Center PowerShellissä**</span><span class="sxs-lookup"><span data-stu-id="60fb5-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="60fb5-114">Lopuksi, jos käyttöliittymässä ei ole kaikkia tarvitsemiasi asetuksia, voit [luoda mukautetun arkaluonteisen tietotyypin Security & Compliance Center PowerShell -toiminnolla.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="60fb5-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="60fb5-115">Aloittamalla XML-tiedostosta voit käyttää kaikkia käytettävissä olevia vaihtoehtoja.</span><span class="sxs-lookup"><span data-stu-id="60fb5-115">By starting with an XML file, you can use every option available.</span></span>
