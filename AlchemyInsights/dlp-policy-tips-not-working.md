---
title: DLP Policy Tips ei toimi
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932583"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="c9c76-102">DLP Policy Vihje kysymyksiä</span><span class="sxs-lookup"><span data-stu-id="c9c76-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="c9c76-103">**Tärkeää:** Monet SharePoint Online- ja OneDrive-asiakkaat kontrunaan ovat liiketoiminnan kannalta kriittisiä sovelluksia taustalla suoritettavaa palvelua vastaan.</span><span class="sxs-lookup"><span data-stu-id="c9c76-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="c9c76-104">Näitä ovat sisällön siirto, tietojen menetyksen estäminen (DLP) ja varmuuskopiointiratkaisut.</span><span class="sxs-lookup"><span data-stu-id="c9c76-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="c9c76-105">Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online- ja OneDrive-palvelut ovat erittäin käytettävissä ja luotettavia käyttäjille, jotka ovat riippuvaisia palvelusta enemmän kuin koskaan etätyöskenaarioissa.</span><span class="sxs-lookup"><span data-stu-id="c9c76-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="c9c76-106">Tämän tavoitteen tukemiseksi olemme toteuttaneet tiukemmat rajoitusrajat taustasovelluksille (siirto, DLP ja varmuuskopiointiratkaisut) arkisin päiväsaikaan.</span><span class="sxs-lookup"><span data-stu-id="c9c76-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="c9c76-107">Sinun pitäisi odottaa, että nämä sovellukset saavuttavat hyvin rajallisen läpikävimäisen käyttökerran näinä aikoina.</span><span class="sxs-lookup"><span data-stu-id="c9c76-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="c9c76-108">Alueen ilta- ja viikonloppuaikoina palvelu on kuitenkin valmis käsittelemään huomattavasti suuremman määrän taustasovellusten pyyntöjä.</span><span class="sxs-lookup"><span data-stu-id="c9c76-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="c9c76-109">**DLP-käytäntövihjeitä**</span><span class="sxs-lookup"><span data-stu-id="c9c76-109">**DLP policy tips**</span></span>

<span data-ttu-id="c9c76-110">Kun käytät **DLP-käytäntöjä**, käyttäjille voidaan ilmoittaa **käytäntövirheestä käytäntövihjeiden**kanssa .</span><span class="sxs-lookup"><span data-stu-id="c9c76-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="c9c76-111">Järjestelmänvalvojat voivat määrittää käytäntövihjeitä näytettäväksi testattaessa DLP-käytäntöäan tai käyttäessään käytäntöä täydessä pakotustilassa.</span><span class="sxs-lookup"><span data-stu-id="c9c76-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="c9c76-112">Voit määrittää DLP-käytännön käytännön vinkkejä suojaus- ja yhteensopivuuskeskuksessa täydessä pakotustilassa seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="c9c76-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="c9c76-113">Varmista, että käytäntövihjeet on **otettu käyttöön** DLP-säännössä noudattamalla [seuraavia](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)ohjeita.</span><span class="sxs-lookup"><span data-stu-id="c9c76-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="c9c76-114">Varmista, että **sisältösi vastaa** **tässä** artikkelissa kuvattua [sääntöä.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="c9c76-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="c9c76-115">Käytäntövihjeet näkyvät sekä OWAssa että Outlookissa.</span><span class="sxs-lookup"><span data-stu-id="c9c76-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="c9c76-116">Kun käytät **Outlook 2013:a tai uudempaa,** käytäntövihjeet näkyvät kuitenkin vain tietyissä olosuhteissa.</span><span class="sxs-lookup"><span data-stu-id="c9c76-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="c9c76-117">Nämä ehdot on lueteltu tässä: [Outlook 2013:n tai uudemman tuetut ehdot käytäntövihjeiden näyttämistä varten](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="c9c76-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="c9c76-118">Lisätietoja DLP-käytäntövihjeissä on kohdassa [DLP-käytäntöjen käytäntövihjeiden näyttäminen](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="c9c76-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  