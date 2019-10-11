---
title: Juuttunut Lähtevät-kansioon suurten liitteiden vuoksi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441303"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="08757-102">Lähtevät-kansioon juuttuneen viestin korjaaminen</span><span class="sxs-lookup"><span data-stu-id="08757-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="08757-103">Microsoft suosittelee, että aloitat suorittamalla skenaarion ["Minulla on ongelmia Sähkö posti viestien lähettämisessä, vastaanottamisessa tai etsimisessä"](https://aka.ms/SaRA-OutlookSendReceive) [Microsoftin tuki-ja palautus avustaja](https://diagnostics.office.com/#/) työkalussa.</span><span class="sxs-lookup"><span data-stu-id="08757-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="08757-104">Kun viesti juuttuu Lähtevät-kansioon, todennäköiset syyt ovat seuraavat:</span><span class="sxs-lookup"><span data-stu-id="08757-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="08757-105">Suuret liitteet.</span><span class="sxs-lookup"><span data-stu-id="08757-105">Large attachments.</span></span>
- <span data-ttu-id="08757-106">**Lähetä heti, kun yhteys on muodostettu** -vaihto ehto ei ole käytössä.</span><span class="sxs-lookup"><span data-stu-id="08757-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="08757-107">Suurten liitteiden poistaminen:</span><span class="sxs-lookup"><span data-stu-id="08757-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="08757-108">Valitse Outlookissa **Lähetä tai vastaanota** > **työ offline-tilassa**.</span><span class="sxs-lookup"><span data-stu-id="08757-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="08757-109">Valitse siirtymis ruudussa **lähtevät-ruutu**.</span><span class="sxs-lookup"><span data-stu-id="08757-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="08757-110">Täältä voit:</span><span class="sxs-lookup"><span data-stu-id="08757-110">From here, you can:</span></span> 
    - <span data-ttu-id="08757-111">Poista viesti (valitse se ja valitse sitten **Poista**).</span><span class="sxs-lookup"><span data-stu-id="08757-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="08757-112">Vedä viesti Luonnokset-kansioon, avaa se kaksoisnapsauttamalla sitä ja poista liite valitsemalla se ja valitsemalla sitten **Poista**).</span><span class="sxs-lookup"><span data-stu-id="08757-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="08757-113">Jos näyttöön tulee virhe sanoma, jonka mukaan Outlook yrittää välittää viestiä, Sulje Outlook.</span><span class="sxs-lookup"><span data-stu-id="08757-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="08757-114">Poistuminen voi kestää hetken.</span><span class="sxs-lookup"><span data-stu-id="08757-114">It may take a few moments to exit.</span></span> <span data-ttu-id="08757-115">Jos Outlook ei sulkeua, paina Ctrl + Alt + Delete ja valitse **Käynnistä Tehtävienhallinta**.</span><span class="sxs-lookup"><span data-stu-id="08757-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="08757-116">Valitse Tehtävienhallinnassa **prosessit** -väli lehti, Vieritä alaspäin Outlook. exe-kohtaan ja valitse **Lopeta prosessi**.</span><span class="sxs-lookup"><span data-stu-id="08757-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="08757-117">Kun Outlook sulkeutuu, käynnistä se uudelleen ja toista vaiheet 2 ja 3.</span><span class="sxs-lookup"><span data-stu-id="08757-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="08757-118">Kun olet poistanut liitteen, Jatka työskentelyä verkossa valitsemalla **Lähetä tai vastaanota** > **offline-tilassa** .</span><span class="sxs-lookup"><span data-stu-id="08757-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="08757-119">Viestit jäävät myös Lähtevät-kansioon, kun napsautat **Lähetä**-painiketta, mutta et ole yhteydessä.</span><span class="sxs-lookup"><span data-stu-id="08757-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="08757-120">Valitse **Lähetä tai vastaanota** ja katso **työ offline** -painiketta.</span><span class="sxs-lookup"><span data-stu-id="08757-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="08757-121">Jos se on sininen, yhteyteemme katkeaa.</span><span class="sxs-lookup"><span data-stu-id="08757-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="08757-122">Valitse se yhdistääksesi (painike muuttuu valkoiseksi) ja napsauta **Lähetä kaikki**.</span><span class="sxs-lookup"><span data-stu-id="08757-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="08757-123">Lähetyksen ottaminen käyttöön **heti, kun yhteys on muodostettu**:</span><span class="sxs-lookup"><span data-stu-id="08757-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="08757-124">Valitse **tiedoston** > **Asetukset** >  **Advanced**.</span><span class="sxs-lookup"><span data-stu-id="08757-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="08757-125">Valitse **Lähetä ja vastaanota** -osiossa **Lähetä heti, kun yhteys on muodostettu**, ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="08757-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="08757-126">Täydelliset tiedot ovat kohdassa:</span><span class="sxs-lookup"><span data-stu-id="08757-126">For full details see:</span></span>
- [<span data-ttu-id="08757-127">Video: jumissa olevan sähkö postin lähettäminen tai poistaminen</span><span class="sxs-lookup"><span data-stu-id="08757-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="08757-128">Sähkö posti pysyy Lähtevät-kansiossa, kunnes voit aloittaa lähetys-ja vastaanotto toiminnon manuaalisesti Outlookissa</span><span class="sxs-lookup"><span data-stu-id="08757-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
