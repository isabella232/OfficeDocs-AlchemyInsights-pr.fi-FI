---
title: Ota selvää, kuka on määrittänyt edelleenlähetystä postilaatikossa ja miten
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429612"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="54742-102">Ota selvää, kuka on määrittänyt edelleenlähetystä postilaatikossa ja miten</span><span class="sxs-lookup"><span data-stu-id="54742-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="54742-103">Jos postilaatikossa on määritetty ulkoinen edelleenlähetys, toiminta valvotaan osana Set-Mailbox cmdlet-komentoa.</span><span class="sxs-lookup"><span data-stu-id="54742-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="54742-104">Näin löydät toiminnon valvontalokista:</span><span class="sxs-lookup"><span data-stu-id="54742-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="54742-105">Siirry [Office 365:n tietoturva- & yhteensopivuuskeskukseen.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="54742-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="54742-106">Valitse **Haun** >  **valvontalokihaku.**</span><span class="sxs-lookup"><span data-stu-id="54742-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="54742-107">Jos näet ilmoituksen, että valvonta on syytä ottaa käyttöön, ota se käyttöön nyt.</span><span class="sxs-lookup"><span data-stu-id="54742-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="54742-108">Jos tätä ominaisuutta ei ole otettu käyttöön, hakutulokset eivät voi hakea tietoja aiemmista päivämääristä.</span><span class="sxs-lookup"><span data-stu-id="54742-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="54742-109">Varmista, että **Toiminnot-kentän** **arvoksi on määritetty Näytä kaikkien toimintojen** tulokset (oletus).</span><span class="sxs-lookup"><span data-stu-id="54742-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="54742-110">Määritä päivämääräalue.</span><span class="sxs-lookup"><span data-stu-id="54742-110">Specify the date range.</span></span> <span data-ttu-id="54742-111">Käyttäjänimeä ei tarvitse määrittää.</span><span class="sxs-lookup"><span data-stu-id="54742-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="54742-112">Valitse **Hae.**</span><span class="sxs-lookup"><span data-stu-id="54742-112">Select **Search**.</span></span> <span data-ttu-id="54742-113">Toiminnot näkyvät **Tulokset-kohdassa.**</span><span class="sxs-lookup"><span data-stu-id="54742-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="54742-114">Valitse **Suodata** tulokset ja kirjoita sitten **Aseta-postilaatikko** **Toimintasuodatin-kenttään.**</span><span class="sxs-lookup"><span data-stu-id="54742-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="54742-115">Tämä palauttaa kaikki **Set-Mailbox-toiminnot.**</span><span class="sxs-lookup"><span data-stu-id="54742-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="54742-116">Voit tarkastella tietoja valitsemalla aktiviteetin ja valitsemalla sitten **Lisätietoja.**</span><span class="sxs-lookup"><span data-stu-id="54742-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="54742-117">**Parametrit-kohdassa** näet postilaatikossa olevan edelleenlähetyssähköpostiosoitteen.</span><span class="sxs-lookup"><span data-stu-id="54742-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="54742-118">Käyttäjätunnus **edustaa** käyttäjää, joka on määrittänyt postilaatikossa ulkoisen edelleenlähetyspalvelun.</span><span class="sxs-lookup"><span data-stu-id="54742-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="54742-119">Lisätietoja on ohjeaiheessa Office [365:n valvontalokista etsiminen yleisimpiä skenaarioita varten.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="54742-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>