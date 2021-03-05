---
title: Poistettujen tapahtumien valvontalokien lukeminen
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481558"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="b0722-102">Poistettujen tapahtumien valvontalokien lukeminen</span><span class="sxs-lookup"><span data-stu-id="b0722-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="b0722-103">Voit tehdä tämän näin:</span><span class="sxs-lookup"><span data-stu-id="b0722-103">Here's how to do this:</span></span>

1. <span data-ttu-id="b0722-104">Siirry [Office 365:n tietoturva- & yhteensopivuuskeskukseen.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="b0722-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="b0722-105">Valitse **Haun**  >  [**valvontalokihaku.**](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="b0722-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="b0722-106">Jos huomaat, että ominaisuus on syytä ottaa käyttöön, ota se käyttöön nyt.</span><span class="sxs-lookup"><span data-stu-id="b0722-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="b0722-107">Jos ominaisuutta ei ole otettu käyttöön, hakutulokset eivät voi hakea tietoja aiemmista päivämääristä.</span><span class="sxs-lookup"><span data-stu-id="b0722-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="b0722-108">Valitse **Toiminnot** ja etsi **exchange-postilaatikon toiminnot.**</span><span class="sxs-lookup"><span data-stu-id="b0722-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="b0722-109">Valitse **Poistetut-kansiosta Poistetut-kansio** ja **Siirretty viestit Poistetut-kansion** asetuksiin.</span><span class="sxs-lookup"><span data-stu-id="b0722-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="b0722-110">Kun olet valmis, pienennä Toiminnot-ruutu napsauttamalla ruudun **ulkopuolella.**</span><span class="sxs-lookup"><span data-stu-id="b0722-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="b0722-111">Määritä päivämääräalue ja valitse sitten **Käyttäjät-ruudussa** sen käyttäjän käyttäjänimi, jonka haluat tutkia.</span><span class="sxs-lookup"><span data-stu-id="b0722-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="b0722-112">Voit valita useamman kuin yhden käyttäjän kerrallaan.</span><span class="sxs-lookup"><span data-stu-id="b0722-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="b0722-113">Valitse **Hae.**</span><span class="sxs-lookup"><span data-stu-id="b0722-113">Select **Search**.</span></span> <span data-ttu-id="b0722-114">Toiminnot näkyvät **Tulokset-kohdassa.**</span><span class="sxs-lookup"><span data-stu-id="b0722-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="b0722-115">Voit tarkastella tietoja valitsemalla aktiviteetin ja valitsemalla sitten **Lisätietoja.**</span><span class="sxs-lookup"><span data-stu-id="b0722-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="b0722-116">Lisätietoja poistetusta kohteesta, kuten aiherivi ja kohteen sijainti, kun se poistettiin, näytetään **AffectedItems-kentässä.**</span><span class="sxs-lookup"><span data-stu-id="b0722-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="b0722-117">Poistettuja kohteita ei voi palauttaa valvontalokitoiminnolla.</span><span class="sxs-lookup"><span data-stu-id="b0722-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="b0722-118">Lisätietoja poistettujen kohteiden palauttamisesta on kohdassa [Poistettujen kohteiden tai sähköpostiviestien palauttaminen Outlook Web Appissa.](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="b0722-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="b0722-119">Lisätietoja on ohjeaiheessa Office [365:n valvontalokista etsiminen yleisimpiä skenaarioita varten.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="b0722-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
