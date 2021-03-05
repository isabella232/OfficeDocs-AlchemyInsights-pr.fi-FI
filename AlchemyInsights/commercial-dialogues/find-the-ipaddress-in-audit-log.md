---
title: IP-osoitteen etsiminen valvontalokista
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481719"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="c2131-102">IP-osoitteen etsiminen valvontalokista</span><span class="sxs-lookup"><span data-stu-id="c2131-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="c2131-103">Käyttäjän tai järjestelmänvalvojan suorittamaa toimintaa vastaava IP-osoite näkyy valvontalokeissa.</span><span class="sxs-lookup"><span data-stu-id="c2131-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="c2131-104">Asiakkaan tiedot kirjataan myös lokiin.</span><span class="sxs-lookup"><span data-stu-id="c2131-104">The client information is also logged.</span></span> <span data-ttu-id="c2131-105">Voit tunnistaa IP-osoitteen näin:</span><span class="sxs-lookup"><span data-stu-id="c2131-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="c2131-106">Siirry [Office 365:n tietoturva- & yhteensopivuuskeskukseen.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="c2131-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="c2131-107">Valitse **Haun**  >  **[valvontalokihaku.](https://go.microsoft.com/fwlink/?linkid=2103759)**</span><span class="sxs-lookup"><span data-stu-id="c2131-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="c2131-108">Jos näet ilmoituksen, että valvonta on syytä ottaa käyttöön, ota se käyttöön nyt.</span><span class="sxs-lookup"><span data-stu-id="c2131-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="c2131-109">Jos tätä ominaisuutta ei ole otettu käyttöön, hakutulokset eivät voi hakea tietoja aiemmista päivämääristä.</span><span class="sxs-lookup"><span data-stu-id="c2131-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="c2131-110">Jos olet kiinnostunut tietystä aktiviteetista, valitse se **Toiminnot-luettelosta.** Muussa tapauksessa kaikki toiminnot palautetaan oletusarvoisesti valitulle käyttäjälle.</span><span class="sxs-lookup"><span data-stu-id="c2131-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="c2131-111">Huomaa, että tietyt toiminnot eivät ehkä ole käytettävissä **Toiminnot-valikossa;** Nämä valvontakohteet palautetaan kuitenkin, jos **Näytä kaikkien toimintojen** tulokset on valittuna (oletusasetus).</span><span class="sxs-lookup"><span data-stu-id="c2131-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="c2131-112">Määritä päivämääräalue ja valitse **Käyttäjät-kentässä** sen käyttäjän käyttäjänimi, jonka haluat tutkia.</span><span class="sxs-lookup"><span data-stu-id="c2131-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="c2131-113">Valitse **Hae.**</span><span class="sxs-lookup"><span data-stu-id="c2131-113">Select **Search**.</span></span> <span data-ttu-id="c2131-114">Toiminnot näkyvät **Tulokset-kohdassa.**</span><span class="sxs-lookup"><span data-stu-id="c2131-114">The activities appear under **Results**.</span></span> <span data-ttu-id="c2131-115">Näet kunkin toiminnon IP-osoitteen.</span><span class="sxs-lookup"><span data-stu-id="c2131-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="c2131-116">Voit tarkastella tietoja valitsemalla aktiviteetin ja valitsemalla **sitten Lisätietoja.**</span><span class="sxs-lookup"><span data-stu-id="c2131-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="c2131-117">Lisätietoja on ohjeaiheessa Office [365:n valvontalokista etsiminen yleisimpiä skenaarioita varten.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="c2131-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>