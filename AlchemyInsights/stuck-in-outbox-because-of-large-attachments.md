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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232627"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="9498c-102">Lähtevät-kansioon jumissa olevien viestien korjaaminen</span><span class="sxs-lookup"><span data-stu-id="9498c-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="9498c-103">Microsoft suosittelee, että aloitat suorittamalla ongelman sisältävän koneen [Microsoftin tuki- ja palautusavustajatyökalun](https://diagnostics.office.com/#/) [skenaarion "Minulla on ongelmia sähköpostiviestien lähettämisessä, vastaanottamisessa tai etsimisen](https://aka.ms/SaRA-OutlookSendReceive) etsinnässä".</span><span class="sxs-lookup"><span data-stu-id="9498c-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="9498c-104">Kun viesti juuttuu Lähtevät-kansioon, todennäköisin syy on suuri liite tai "Lähetä heti, kun yhteys" -vaihtoehto ei ole käytössä.</span><span class="sxs-lookup"><span data-stu-id="9498c-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="9498c-105">**Suuren liitteen irrottaminen**</span><span class="sxs-lookup"><span data-stu-id="9498c-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="9498c-106">Valitse **Lähetä tai vastaanota** > **työ offline-tilassa**.</span><span class="sxs-lookup"><span data-stu-id="9498c-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="9498c-107">Valitse siirtymisruudussa **Lähtevät**.</span><span class="sxs-lookup"><span data-stu-id="9498c-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="9498c-108">Täältä voit:</span><span class="sxs-lookup"><span data-stu-id="9498c-108">From here, you can:</span></span> 
    - <span data-ttu-id="9498c-109">Poista viesti.</span><span class="sxs-lookup"><span data-stu-id="9498c-109">Delete the message.</span></span> <span data-ttu-id="9498c-110">Valitse se ja valitse **Poista**.</span><span class="sxs-lookup"><span data-stu-id="9498c-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="9498c-111">Vedä viesti **luonnoskansioon,** avaa viesti kaksoisnapsauttamalla sitä ja poista liite (napsauta sitä ja valitse **Poista**).</span><span class="sxs-lookup"><span data-stu-id="9498c-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="9498c-112">Jos virhe ilmoittaa, että Outlook yrittää lähettää viestin, sulje Outlook.</span><span class="sxs-lookup"><span data-stu-id="9498c-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="9498c-113">Se voi kestää hetken poistua.</span><span class="sxs-lookup"><span data-stu-id="9498c-113">It may take a few moments to exit.</span></span> <span data-ttu-id="9498c-114">Jos Outlook ei sulkeudu, paina **Näppäinyhdistelmää Ctrl+Alt+Delete** ja valitse **Käynnistä Tehtävienhallinta**.</span><span class="sxs-lookup"><span data-stu-id="9498c-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="9498c-115">Valitse Tehtävienhallinnassa **Prosessit-välilehti,** vieritä alas outlook.exe-tiedostoon ja valitse **Lopeta prosessi**.</span><span class="sxs-lookup"><span data-stu-id="9498c-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="9498c-116">Kun Outlook sulkeutuu, käynnistä Outlook uudelleen ja toista vaiheet 2-3.</span><span class="sxs-lookup"><span data-stu-id="9498c-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="9498c-117">Kun olet poistanut liitteen, poista painikkeen valinta ja jatka työskentelyä verkossa valitsemalla **Lähetä tai vastaanota** > **offline-tila.**</span><span class="sxs-lookup"><span data-stu-id="9498c-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="9498c-118">Viestit juuttuvat myös Lähtevät-kansioon, kun valitset **Lähetä**, mutta et ole yhteydessä.</span><span class="sxs-lookup"><span data-stu-id="9498c-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="9498c-119">Valitse **Lähetä tai vastaanota** ja katso **Offline-tila-painiketta.**</span><span class="sxs-lookup"><span data-stu-id="9498c-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="9498c-120">Jos se on sininen, yhteys katkeaa.</span><span class="sxs-lookup"><span data-stu-id="9498c-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="9498c-121">Muodosta yhteys napsauttamalla sitä (painike muuttuu valkoiseksi) ja valitse **Lähetä kaikki**.</span><span class="sxs-lookup"><span data-stu-id="9498c-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="9498c-122">**Ota lähetä käyttöön heti, kun yhteys on muodostettu**</span><span class="sxs-lookup"><span data-stu-id="9498c-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="9498c-123">Valitse Tiedosto-välilehdessä **Asetukset**.</span><span class="sxs-lookup"><span data-stu-id="9498c-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="9498c-124">Valitse Outlookin asetukset -valintaikkunassa **Lisäasetukset**.</span><span class="sxs-lookup"><span data-stu-id="9498c-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="9498c-125">Ota Lähetä heti, **kun yhteys on muodostettu,** valitsemalla Lähetä ja vastaanota -osassa .</span><span class="sxs-lookup"><span data-stu-id="9498c-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="9498c-126">Valitse **OK**.</span><span class="sxs-lookup"><span data-stu-id="9498c-126">Click **OK**.</span></span>
 
<span data-ttu-id="9498c-127">Lisätietoja on kohdassa:</span><span class="sxs-lookup"><span data-stu-id="9498c-127">For full details, see:</span></span>
- [<span data-ttu-id="9498c-128">Video: Jumittun sähköpostin lähettäminen tai poistaminen</span><span class="sxs-lookup"><span data-stu-id="9498c-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="9498c-129">Sähköposti pysyy Lähtevät-kansiossa, kunnes käynnistät lähetys- ja vastaanottotoiminnon manuaalisesti Outlookissa</span><span class="sxs-lookup"><span data-stu-id="9498c-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
