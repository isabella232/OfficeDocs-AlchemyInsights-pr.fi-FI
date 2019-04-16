---
title: DLP on ehkä mukautettu tyyppi
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: cd5bac5efe3a16d32f9b695c8cb452a1eaa3a796
ms.sourcegitcommit: e87b3f691444db3b9f460c9a3109146dc7ad4f80
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2019
ms.locfileid: "31872318"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="af1b8-102">DLP on ehkä mukautettu tyyppi</span><span class="sxs-lookup"><span data-stu-id="af1b8-102">DLP might need a custom type</span></span>

<span data-ttu-id="af1b8-103">Tietojen menetyksen estäminen (DLP) käytännön voit tunnistaa ja suojaa organisaatiosi luottamukselliset tiedot.</span><span class="sxs-lookup"><span data-stu-id="af1b8-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="af1b8-104">Joissakin tilanteissa saatat joutua luoda omia **mukautettuja** luottamuksellisia tietoja organisaation tietojen suojaamiseksi.</span><span class="sxs-lookup"><span data-stu-id="af1b8-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="af1b8-105">Esimerkiksi organisaation täytyy ehkä tunnistaa ja suojata työntekijätunnusten tai muita tietoja muodossa joitakin erityisiä että org. Jos näin on, katso lisätietoja seuraavista artikkeleista.</span><span class="sxs-lookup"><span data-stu-id="af1b8-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span> 
  
 <span data-ttu-id="af1b8-106">**Mukauttaa valmiin luottamuksellisten tietojen tyyppi**</span><span class="sxs-lookup"><span data-stu-id="af1b8-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="af1b8-107">Jos sisäinen luottamuksellisten tietojen tyyppi tarpeittesi kanssa muutaman tweaks, voit [mukauttaa valmiin luottamuksellisten tietojen tyyppi](https://docs.microsoft.com/en-us/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="af1b8-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/en-us/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="af1b8-108">Voit esimerkiksi lisätä tai poistaa avainsanoja, tai lisätä tai poistaa todisteisiin, kuten päivämäärän tai osoite.</span><span class="sxs-lookup"><span data-stu-id="af1b8-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="af1b8-109">**Luo mukautettu luottamuksellisten tietojen tyyppi**</span><span class="sxs-lookup"><span data-stu-id="af1b8-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="af1b8-110">Mutta jos täytyy tunnistaa ja suojaa arkaluonteisia tietoja erilaisella kokonaan, voit [luoda mukautetun luottamuksellisten tietojen](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type) suojaus & Compliance Centerin käyttöliittymässä.</span><span class="sxs-lookup"><span data-stu-id="af1b8-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span> 
  
<span data-ttu-id="af1b8-111">**Luoda mukautettuja luottamuksellisten tietojen suojaus & Compliance Centerin PowerShell-**</span><span class="sxs-lookup"><span data-stu-id="af1b8-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="af1b8-112">Lopuksi, jos Käyttöliittymä ei tarjoa kaikki tarvittavat asetukset, voit [luoda mukautetun arkaluontoisten tietojen suojaus & Compliance Centerin PowerShell](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="af1b8-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="af1b8-113">Alkaen XML-tiedostoon, voit käyttää jokaisen asetuksen.</span><span class="sxs-lookup"><span data-stu-id="af1b8-113">By starting with an XML file, you can use every option available.</span></span>

    
