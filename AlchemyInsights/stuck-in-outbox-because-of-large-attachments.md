---
title: Jumissa Lähtevät-kansiossa suurten liitteiden vuoksi
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
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241249"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="2987e-102">Lähtevät-kansioon jumissa olevien viestien korjaaminen</span><span class="sxs-lookup"><span data-stu-id="2987e-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="2987e-103">Microsoft suosittelee, että aloitat suorittamalla [Microsoftin tuki- ja palautusavustajatyökalun](https://diagnostics.office.com/#/) skenaarion ["Minulla on ongelmia sähköpostiviestien lähettämisessä, vastaanottamisessa tai etsimisen etsinnässä".](https://aka.ms/SaRA-OutlookSendReceive)</span><span class="sxs-lookup"><span data-stu-id="2987e-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="2987e-104">Kun viesti juuttuu Lähtevät-kansioon, todennäköisin syy on suuri liite tai "Lähetä heti, kun yhteys" -vaihtoehto ei ole käytössä.</span><span class="sxs-lookup"><span data-stu-id="2987e-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="2987e-105">**Suuren liitteen irrottaminen**</span><span class="sxs-lookup"><span data-stu-id="2987e-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="2987e-106">Valitse Outlookissa **Lähetä tai vastaanota** > **työ offline-tilassa**.</span><span class="sxs-lookup"><span data-stu-id="2987e-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="2987e-107">Valitse siirtymisruudussa **Lähtevät**.</span><span class="sxs-lookup"><span data-stu-id="2987e-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="2987e-108">Täältä voit:</span><span class="sxs-lookup"><span data-stu-id="2987e-108">From here, you can:</span></span> 
    - <span data-ttu-id="2987e-109">Poista viesti (valitse se ja valitse sitten **Poista**).</span><span class="sxs-lookup"><span data-stu-id="2987e-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="2987e-110">Vedä viesti Luonnokset-kansioon, avaa se kaksoisnapsauttamalla sitä, poista liite ja valitse se ja valitse sitten **Poista**).</span><span class="sxs-lookup"><span data-stu-id="2987e-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="2987e-111">Jos näyttöön tulee virhe, jonka mukaan Outlook yrittää lähettää viestin, sulje Outlook.</span><span class="sxs-lookup"><span data-stu-id="2987e-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="2987e-112">Se voi kestää hetken poistua.</span><span class="sxs-lookup"><span data-stu-id="2987e-112">It may take a few moments to exit.</span></span> <span data-ttu-id="2987e-113">Jos Outlook ei sulkeudu, paina Näppäinyhdistelmää Ctrl+Alt+Delete ja valitse **Aloita Tehtävienhallinta**.</span><span class="sxs-lookup"><span data-stu-id="2987e-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="2987e-114">Valitse Tehtävienhallinnassa **Prosessit-välilehti,** vieritä alas outlook.exe-tiedostoon ja valitse **Lopeta prosessi**.</span><span class="sxs-lookup"><span data-stu-id="2987e-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="2987e-115">Kun Outlook sulkeutuu, käynnistä se uudelleen ja toista vaiheet 2 ja 3.</span><span class="sxs-lookup"><span data-stu-id="2987e-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="2987e-116">Kun olet poistanut liitteen, jatka työskentelyä verkossa valitsemalla **Lähetä tai vastaanota** > **offline-tilassa.**</span><span class="sxs-lookup"><span data-stu-id="2987e-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="2987e-117">Viestit juuttuvat myös Lähtevät-kansioon, kun valitset **Lähetä**, mutta et ole yhteydessä.</span><span class="sxs-lookup"><span data-stu-id="2987e-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="2987e-118">Valitse **Lähetä tai vastaanota** ja katso **Offline-tila-painiketta.**</span><span class="sxs-lookup"><span data-stu-id="2987e-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="2987e-119">Jos se on sininen, yhteys katkeaa.</span><span class="sxs-lookup"><span data-stu-id="2987e-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="2987e-120">Muodosta yhteys napsauttamalla sitä (painike muuttuu valkoiseksi) ja valitse **Lähetä kaikki**.</span><span class="sxs-lookup"><span data-stu-id="2987e-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="2987e-121">**Ota lähetä käyttöön heti, kun yhteys on muodostettu**</span><span class="sxs-lookup"><span data-stu-id="2987e-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="2987e-122">Valitse Tiedosto-välilehdessä **Asetukset**.</span><span class="sxs-lookup"><span data-stu-id="2987e-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="2987e-123">Valitse Outlookin asetukset -valintaikkunassa **Lisäasetukset**.</span><span class="sxs-lookup"><span data-stu-id="2987e-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="2987e-124">Ota Lähetä heti, **kun yhteys on muodostettu,** valitsemalla Lähetä ja vastaanota -osassa .</span><span class="sxs-lookup"><span data-stu-id="2987e-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="2987e-125">Valitse **OK**.</span><span class="sxs-lookup"><span data-stu-id="2987e-125">Click **OK**.</span></span>
 
<span data-ttu-id="2987e-126">Lisätietoja on kohdassa:</span><span class="sxs-lookup"><span data-stu-id="2987e-126">For full details, see:</span></span>
- [<span data-ttu-id="2987e-127">Video: Jumittun sähköpostin lähettäminen tai poistaminen</span><span class="sxs-lookup"><span data-stu-id="2987e-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="2987e-128">Sähköposti pysyy Lähtevät-kansiossa, kunnes käynnistät lähetys- ja vastaanottotoiminnon manuaalisesti Outlookissa</span><span class="sxs-lookup"><span data-stu-id="2987e-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
