---
title: Saapuneet-kansion säännöille suoritettujen tapahtumien etsiminen
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481718"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="c3741-102">Saapuneet-kansion säännöille suoritettujen tapahtumien etsiminen</span><span class="sxs-lookup"><span data-stu-id="c3741-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="c3741-103">Kun Saapuneet-kansion sääntöjä luodaan, muutetaan tai poistetaan, tapahtumat tallennetaan valvontalokiin.</span><span class="sxs-lookup"><span data-stu-id="c3741-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="c3741-104">Voit tarkistaa ne näin:</span><span class="sxs-lookup"><span data-stu-id="c3741-104">Here's how to review them:</span></span>

1. <span data-ttu-id="c3741-105">Siirry [Office 365:n tietoturva- & yhteensopivuuskeskukseen.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="c3741-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="c3741-106">Valitse > valvontalokihaku.</span><span class="sxs-lookup"><span data-stu-id="c3741-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c3741-107">Jos näet ilmoituksen, että valvonta on syytä ottaa käyttöön, ota se käyttöön nyt.</span><span class="sxs-lookup"><span data-stu-id="c3741-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="c3741-108">Jos tätä ominaisuutta ei ole otettu käyttöön, hakutulokset eivät voi hakea tietoja aiemmista päivämääristä.</span><span class="sxs-lookup"><span data-stu-id="c3741-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="c3741-109">Valitse Toiminnot-kenttä, etsi Exchange-postilaatikon toiminnot ja valitse sitten New-InboxRule luo Saapuneet-kansion sääntö Outlook Web Appista.</span><span class="sxs-lookup"><span data-stu-id="c3741-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="c3741-110">Kun olet valmis, pienennä Toiminnot-ruutu napsauttamalla ruudun ulkopuolella.</span><span class="sxs-lookup"><span data-stu-id="c3741-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="c3741-111">Määritä päivämääräalue ja valitse sitten Käyttäjät-kentässä sen käyttäjän käyttäjänimi, jonka haluat tutkia.</span><span class="sxs-lookup"><span data-stu-id="c3741-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="c3741-112">Voit valita useamman kuin yhden käyttäjän kerrallaan.</span><span class="sxs-lookup"><span data-stu-id="c3741-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="c3741-113">Valitse Hae.</span><span class="sxs-lookup"><span data-stu-id="c3741-113">Select Search.</span></span> <span data-ttu-id="c3741-114">Toiminnot näkyvät Tulokset-kohdassa.</span><span class="sxs-lookup"><span data-stu-id="c3741-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="c3741-115">Voit tarkastella tietoja valitsemalla aktiviteetin ja valitsemalla sitten Lisätietoja.</span><span class="sxs-lookup"><span data-stu-id="c3741-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="c3741-116">Parametrit-osassa näet säännön nimen, ehdot ja säännön toiminnot.</span><span class="sxs-lookup"><span data-stu-id="c3741-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="c3741-117">Lisätietoja on ohjeaiheessa Office 365:n valvontalokista etsiminen yleisimpiä skenaarioita varten.</span><span class="sxs-lookup"><span data-stu-id="c3741-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>