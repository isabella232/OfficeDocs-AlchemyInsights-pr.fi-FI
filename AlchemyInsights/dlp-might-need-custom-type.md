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
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932655"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="81644-102">DLP saattaa tarvita mukautetun tyypin</span><span class="sxs-lookup"><span data-stu-id="81644-102">DLP might need a custom type</span></span>

<span data-ttu-id="81644-103">**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan.</span><span class="sxs-lookup"><span data-stu-id="81644-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="81644-104">Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut.</span><span class="sxs-lookup"><span data-stu-id="81644-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="81644-105">Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.</span><span class="sxs-lookup"><span data-stu-id="81644-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="81644-106">Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan.</span><span class="sxs-lookup"><span data-stu-id="81644-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="81644-107">Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina.</span><span class="sxs-lookup"><span data-stu-id="81644-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="81644-108">Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.</span><span class="sxs-lookup"><span data-stu-id="81644-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="81644-109">**DLP voi vaatia mukautetun tietotyypin**</span><span class="sxs-lookup"><span data-stu-id="81644-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="81644-110">DLP (Data Loss Prevention) -käytännön avulla voit tunnistaa ja suojata organisaation arkaluonteisia tietoja.</span><span class="sxs-lookup"><span data-stu-id="81644-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="81644-111">Joissakin tilanteissa sinun on ehkä luotava oma **mukautettu** tietotyyppi organisaatiosi tietojen suojaamiseksi.</span><span class="sxs-lookup"><span data-stu-id="81644-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="81644-112">Organisaatiosi on esimerkiksi ehkä tunnistettava ja suojattava työntekijätunnusten tai muiden tietojen tunnistamisessa organisaatiosi tietyssä muodossa. Jos näin on, katso lisätietoja seuraavista artikkeleista.</span><span class="sxs-lookup"><span data-stu-id="81644-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="81644-113">**Sisäisen arkaluonteisen tietotyypin mukauttaminen**</span><span class="sxs-lookup"><span data-stu-id="81644-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="81644-114">Jos sisäänrakennettu arkaluonteinen tietotyyppi vastaisi tarpeitasi muutamalla sävyllä, voit [mukauttaa sisäisen arkaluonteisen tietotyypin](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="81644-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="81644-115">Voit esimerkiksi lisätä tai poistaa avainsanoja tai lisätä tai poistaa todisteita, kuten päivämäärän tai osoitteen.</span><span class="sxs-lookup"><span data-stu-id="81644-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="81644-116">**Mukautetun arkaluonteisen tietotyypin luominen**</span><span class="sxs-lookup"><span data-stu-id="81644-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="81644-117">Jos sinun on kuitenkin tunnistettava ja suojattava erityyppiset arkaluonteiset tiedot kokonaan, voit [luoda mukautetun arkaluonteisen tietotyypin](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) Suojaus& Yhteensopivuuskeskuksen käyttöliittymässä.</span><span class="sxs-lookup"><span data-stu-id="81644-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="81644-118">**Mukautetun arkaluonteisen tietotyypin luominen Tietoturva& Compliance Center PowerShellissä**</span><span class="sxs-lookup"><span data-stu-id="81644-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="81644-119">Jos käyttöliittymässä ei ole kaikkia tarvitsemiasi asetuksia, voit [luoda mukautetun arkaluonteisen tietotyypin Tietoturva-& Yhteensopivuuskeskus PowerShellissä](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="81644-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="81644-120">Aloittamalla XML-tiedostosta voit käyttää kaikkia käytettävissä olevia vaihtoehtoja.</span><span class="sxs-lookup"><span data-stu-id="81644-120">By starting with an XML file, you can use every option available.</span></span>
