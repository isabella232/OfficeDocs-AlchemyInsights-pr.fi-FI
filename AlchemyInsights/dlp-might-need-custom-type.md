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
ms.openlocfilehash: 87fcb5c3cc9ccd525265097b66d9d9b3a85c5feb
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977267"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="9b092-102">DLP saattaa tarvita mukautetun tyypin</span><span class="sxs-lookup"><span data-stu-id="9b092-102">DLP might need a custom type</span></span>

<span data-ttu-id="9b092-103">**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat edelleen erittäin saatavilla – lisätietoja on [SharePoint Onlinen tilapäisissä ominaisuusoikaisuissa.](https://aka.ms/ODSPAdjustments)</span><span class="sxs-lookup"><span data-stu-id="9b092-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="9b092-104">**DLP voi vaatia mukautetun tietotyypin**</span><span class="sxs-lookup"><span data-stu-id="9b092-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="9b092-105">DLP (Data Loss Prevention) -käytännön avulla voit tunnistaa ja suojata organisaation arkaluonteisia tietoja.</span><span class="sxs-lookup"><span data-stu-id="9b092-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="9b092-106">Joissakin tilanteissa sinun on ehkä luotava oma **mukautettu** tietotyyppi organisaatiosi tietojen suojaamiseksi.</span><span class="sxs-lookup"><span data-stu-id="9b092-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="9b092-107">Organisaatiosi on esimerkiksi ehkä tunnistettava ja suojattava työntekijätunnusten tai muiden tietojen tunnistamisessa organisaatiosi tietyssä muodossa. Jos näin on, katso lisätietoja seuraavista artikkeleista.</span><span class="sxs-lookup"><span data-stu-id="9b092-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="9b092-108">**Sisäisen arkaluonteisen tietotyypin mukauttaminen**</span><span class="sxs-lookup"><span data-stu-id="9b092-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="9b092-109">Jos sisäänrakennettu arkaluonteinen tietotyyppi vastaisi tarpeitasi muutamalla sävyllä, voit [mukauttaa sisäisen arkaluonteisen tietotyypin](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="9b092-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="9b092-110">Voit esimerkiksi lisätä tai poistaa avainsanoja tai lisätä tai poistaa todisteita, kuten päivämäärän tai osoitteen.</span><span class="sxs-lookup"><span data-stu-id="9b092-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="9b092-111">**Mukautetun arkaluonteisen tietotyypin luominen**</span><span class="sxs-lookup"><span data-stu-id="9b092-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="9b092-112">Jos sinun on kuitenkin tunnistettava ja suojattava erityyppiset arkaluonteiset tiedot kokonaan, voit [luoda mukautetun arkaluonteisen tietotyypin](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) Suojaus& Yhteensopivuuskeskuksen käyttöliittymässä.</span><span class="sxs-lookup"><span data-stu-id="9b092-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="9b092-113">**Mukautetun arkaluonteisen tietotyypin luominen Tietoturva& Compliance Center PowerShellissä**</span><span class="sxs-lookup"><span data-stu-id="9b092-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="9b092-114">Jos käyttöliittymässä ei ole kaikkia tarvitsemiasi asetuksia, voit [luoda mukautetun arkaluonteisen tietotyypin Tietoturva-& Yhteensopivuuskeskus PowerShellissä](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="9b092-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="9b092-115">Aloittamalla XML-tiedostosta voit käyttää kaikkia käytettävissä olevia vaihtoehtoja.</span><span class="sxs-lookup"><span data-stu-id="9b092-115">By starting with an XML file, you can use every option available.</span></span>
