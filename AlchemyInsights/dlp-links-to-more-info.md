---
title: Lisätietoja DLP-ongelmista
ms.author: pebaum
author: pebaum
manager: laurawi
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2447"
- "3200001"
ms.openlocfilehash: 6525cee0555f1ae67b7d4e32445b9a1537d4a804
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932691"
---
# <a name="information-about-dlp-issues"></a><span data-ttu-id="6e889-102">Tietoja DLP-ongelmista</span><span class="sxs-lookup"><span data-stu-id="6e889-102">Information about DLP issues</span></span>

<span data-ttu-id="6e889-103">**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan.</span><span class="sxs-lookup"><span data-stu-id="6e889-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="6e889-104">Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut.</span><span class="sxs-lookup"><span data-stu-id="6e889-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="6e889-105">Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.</span><span class="sxs-lookup"><span data-stu-id="6e889-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="6e889-106">Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan.</span><span class="sxs-lookup"><span data-stu-id="6e889-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="6e889-107">Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina.</span><span class="sxs-lookup"><span data-stu-id="6e889-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="6e889-108">Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.</span><span class="sxs-lookup"><span data-stu-id="6e889-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="6e889-109">**Tietoa DLP-käytännöstä**</span><span class="sxs-lookup"><span data-stu-id="6e889-109">**Information on DLP policy**</span></span>

<span data-ttu-id="6e889-110">DLP-käytännön avulla voit tunnistaa, valvoa ja suojata automaattisesti arkaluonteisia tietoja Office 365:ssä.</span><span class="sxs-lookup"><span data-stu-id="6e889-110">With a DLP policy, you can identify, monitor, and automatically protect sensitive information across Office 365.</span></span>

<span data-ttu-id="6e889-111">Lisätietoja on näissä linkeissä:</span><span class="sxs-lookup"><span data-stu-id="6e889-111">Please visit these links for more information:</span></span>

- [<span data-ttu-id="6e889-112">Yleiskatsaus tietojen menetyksen estämiseen</span><span class="sxs-lookup"><span data-stu-id="6e889-112">Overview of data loss prevention</span></span>](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies)
- [<span data-ttu-id="6e889-113">Mitä arkaluonteiset tietotyypit etsivät</span><span class="sxs-lookup"><span data-stu-id="6e889-113">What the sensitive information types look for</span></span>](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
- [<span data-ttu-id="6e889-114">Mukautetun arkaluonteisen tietotyypin luominen</span><span class="sxs-lookup"><span data-stu-id="6e889-114">Create a custom sensitive information type</span></span>](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)
- [<span data-ttu-id="6e889-115">Sähköposti-ilmoitusten lähettäminen ja käytäntövihjeiden näyttäminen</span><span class="sxs-lookup"><span data-stu-id="6e889-115">Send email notifications and show policy tips</span></span>](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
- [<span data-ttu-id="6e889-116">SharePoint Online -tiedostojen suojaaminen säilytysotsikoilla ja DLP:llä</span><span class="sxs-lookup"><span data-stu-id="6e889-116">Protect SharePoint Online files with retention labels and DLP</span></span>](https://docs.microsoft.com/office365/securitycompliance/protect-sharepoint-online-files-with-office-365-labels-and-dlp)
- [<span data-ttu-id="6e889-117">DLP ja Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="6e889-117">DLP and Microsoft Teams</span></span>](https://docs.microsoft.com/office365/securitycompliance/dlp-microsoft-teams)

<span data-ttu-id="6e889-118">Jos haluat testata tietoja valmiilla tai mukautetulla arkaluonteisella tietotyypillä, käytä **Luokitusten** > **arkaluonteiset tietotyypit**-kohdan **Testaa tyyppi** -vaihtoehtoa.</span><span class="sxs-lookup"><span data-stu-id="6e889-118">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="6e889-119">Lisätietoja on kohdassa [Mukautettujen arkaluonteisten tietotyyppien testaaminen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="6e889-119">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>