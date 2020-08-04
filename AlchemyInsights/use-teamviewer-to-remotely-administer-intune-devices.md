---
title: Intune-laitteiden etähallinta TeamViewerin avulla
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554974"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="1e765-102">Intune-laitteiden etähallinta TeamViewerin avulla</span><span class="sxs-lookup"><span data-stu-id="1e765-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="1e765-103">Intunen hallitsemia laitteita voidaan hallita etänä [TeamViewerin](https://www.teamviewer.com/)avulla.</span><span class="sxs-lookup"><span data-stu-id="1e765-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="1e765-104">Voit hallita Intunen teamviewerin avulla seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="1e765-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="1e765-105">Aloita hankkimalla TeamViewerilta tunnistetiedot, joiden avulla voit määrittää TeamViewer Connectorin Intunessa.</span><span class="sxs-lookup"><span data-stu-id="1e765-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="1e765-106">Näin järjestelmänvalvoja voi kirjoittaa tunnistetiedot TeamViewer Connector -käyttöliittymään Laitteet-kohdassa, joka on kertatoiminto Intunen ja TeamViewer-palvelun välisen yhteyden muodostamiseksi.</span><span class="sxs-lookup"><span data-stu-id="1e765-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="1e765-107">**Osa 1: Istunnon aloittaminen etälaitteella**</span><span class="sxs-lookup"><span data-stu-id="1e765-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="1e765-108">Valitse **Kaikki laitteet -kohdasta**laite, jolla haluat aloittaa etäistunnon.</span><span class="sxs-lookup"><span data-stu-id="1e765-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="1e765-109">Alkaen **... Lisää**, valitse **Uusi etätukiistunto**.</span><span class="sxs-lookup"><span data-stu-id="1e765-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="1e765-110">Valitse **Kyllä,** jos haluat kuitata etäistunnon.</span><span class="sxs-lookup"><span data-stu-id="1e765-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="1e765-111">Kun TeamViewer-palvelu on hyväksynyt Uuden etäistunnon aloittaminen -pyynnön, näet vaihtoehdon **etätuen käynnistäminen** laitteen Yleiskuvaus-ruudun (tai Essentials)-ruudun tietojen alta.</span><span class="sxs-lookup"><span data-stu-id="1e765-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="1e765-112">Laajenna ruutu ja näytä etätuen tila valitsemalla **Näytä lisää.**</span><span class="sxs-lookup"><span data-stu-id="1e765-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="1e765-113">Aloita istunto järjestelmänvalvojan puolella valitsemalla **Aloita etäistunto.**</span><span class="sxs-lookup"><span data-stu-id="1e765-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="1e765-114">Lataa TeamViewer-binaari (Windows) ja valitse **Suorita**.</span><span class="sxs-lookup"><span data-stu-id="1e765-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="1e765-115">**Huomautus** Voit ohittaa minkä tahansa TeamViewer-web-sivustoon avatun verkkoselaimen sivun.</span><span class="sxs-lookup"><span data-stu-id="1e765-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="1e765-116">Kuittaa TeamViewer-sovelluksen pyyntö tehdä muutoksia laitteeseen (vain Windows).</span><span class="sxs-lookup"><span data-stu-id="1e765-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="1e765-117">TeamViewer-sovellus käynnistyy ja sisältää istuntokoodin yhteyden todentamiseksi etälaitteeseen.</span><span class="sxs-lookup"><span data-stu-id="1e765-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="1e765-118">**Osa 2: Etäistuntoon kohdistettuun laitteeseen**</span><span class="sxs-lookup"><span data-stu-id="1e765-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="1e765-119">Avaa Intune-yritysportaali.</span><span class="sxs-lookup"><span data-stu-id="1e765-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="1e765-120">Etsi ilmoitusmerkintä: "IT-järjestelmänvalvoja pyytää tämän laitteen hallintaa etätukiistuntoon" ja valitse ilmoitus.</span><span class="sxs-lookup"><span data-stu-id="1e765-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="1e765-121">Valitse TeamViewer-sovelluksen lataaminen tai TeamViewer-sovelluksen lataamisen kuittaaminen sovelluskaupasta ja valitse **Suorita**.</span><span class="sxs-lookup"><span data-stu-id="1e765-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="1e765-122">**Huomautus** Voit ohittaa minkä tahansa TeamViewer-web-sivustoon avatun verkkoselaimen sivun.</span><span class="sxs-lookup"><span data-stu-id="1e765-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="1e765-123">Kuittaa TeamViewer-sovelluksen pyyntö tehdä muutoksia laitteeseen (vain Windows).</span><span class="sxs-lookup"><span data-stu-id="1e765-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="1e765-124">TeamViewer-sovellus käynnistyy ja sisältää istuntokoodin yhteyden todentamiseksi etälaitteeseen.</span><span class="sxs-lookup"><span data-stu-id="1e765-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="1e765-125">Ponnahdusikkuna kysyy, haluatko sallia istunnon aloittamisen.</span><span class="sxs-lookup"><span data-stu-id="1e765-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="1e765-126">**Huomautus** TeamViewer-palvelun luomat istuntokoodit ovat vain kertakäyttöiset.</span><span class="sxs-lookup"><span data-stu-id="1e765-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="1e765-127">Jos yhteys katkeaa, sinun on</span><span class="sxs-lookup"><span data-stu-id="1e765-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="1e765-128">Sulje TeamViewer-sovelluksen esiintymä etälaitteessa ja järjestelmänvalvojan työasemassa.</span><span class="sxs-lookup"><span data-stu-id="1e765-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="1e765-129">Sulje etälaitteen yritysportaali.</span><span class="sxs-lookup"><span data-stu-id="1e765-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="1e765-130">Aloita uusi "Uusi etätukiistunto" hallintaportaalista.</span><span class="sxs-lookup"><span data-stu-id="1e765-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="1e765-131">Avaa uusi ilmoitus avaamalla etälaitteen yritysportaali uudelleen.</span><span class="sxs-lookup"><span data-stu-id="1e765-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="1e765-132">Lataa ja avaa TeamViewer-sovellus sekä etälaitteessa että järjestelmänvalvojan työasemassa, kuten ennenkin.</span><span class="sxs-lookup"><span data-stu-id="1e765-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>