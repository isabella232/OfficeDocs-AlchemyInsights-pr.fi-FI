---
title: Virta- tai akkukuvake puuttuu Windows 10:ssä
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790545"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="116ef-102">Virta- tai akkukuvake puuttuu Windows 10:ssä</span><span class="sxs-lookup"><span data-stu-id="116ef-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="116ef-103">Jos Windows 10 -laitteessasi (kuten kannettavassa tietokoneessa, tabletissa tai UPS:ään USB:n avulla yhdistetyssä PC-tietokoneessa) on akku, tehtäväpalkissa lähellä kelloa näytetään tavallisesti virta- tai akkukuvake. Esimerkki:</span><span class="sxs-lookup"><span data-stu-id="116ef-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Akkukuvake](media/battery-icon.png)

<span data-ttu-id="116ef-105">Jos et näe tätä kuvaketta, se on voitu piilottaa:</span><span class="sxs-lookup"><span data-stu-id="116ef-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="116ef-106">Siirry kohtaan **[Asetukset > Mukauttaminen > Tehtäväpalkki](ms-settings:taskbar?activationSource=GetHelp)**.</span><span class="sxs-lookup"><span data-stu-id="116ef-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="116ef-107">Valitse ilmoitusalueella **Valitse, mitkä kuvakkeet näkyvät tehtäväpalkissa**.</span><span class="sxs-lookup"><span data-stu-id="116ef-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="116ef-108">Etsi luettelosta **Virta** ja muuta sen valinnaksi **Käytössä**.</span><span class="sxs-lookup"><span data-stu-id="116ef-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![Virtakuvakkeen näyttäminen tehtäväpalkissa](media/power-icon-on.png)

<span data-ttu-id="116ef-110">**Vianmääritys**</span><span class="sxs-lookup"><span data-stu-id="116ef-110">**Troubleshooting**</span></span>

<span data-ttu-id="116ef-111">Jos noudatit yllä olevia ohjeita eikä **Virta**-vaihtopainiketta näy tai se näkyy harmaana, kirjoita tehtäväpalkin hakuruutuun **laitehallinta** ja valitse sitten tulosluettelosta **Laitehallinta**.</span><span class="sxs-lookup"><span data-stu-id="116ef-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="116ef-112">Napsauta **Akut**-kohdassa laitteesi akkua hiiren kakkospainikkeella. Valitse sitten **Poista käytöstä** ja **Kyllä**.</span><span class="sxs-lookup"><span data-stu-id="116ef-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="116ef-113">Odota muutama sekunti, napsauta akkua hiiren kakkospainikkeella ja valitse **Ota käyttöön**.</span><span class="sxs-lookup"><span data-stu-id="116ef-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="116ef-114">Käynnistä laite sitten uudelleen.</span><span class="sxs-lookup"><span data-stu-id="116ef-114">Then restart your device.</span></span>

<span data-ttu-id="116ef-115">Jos noudatit yllä olevia ohjeita eikä akkukuvaketta näy tehtäväpalkissa, kirjoita tehtäväpalkin hakuruutuun **tehtävien hallinta** ja valitse sitten tulosluettelosta **Tehtävien hallinta**.</span><span class="sxs-lookup"><span data-stu-id="116ef-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="116ef-116">Napsauta **Prosessit**-välilehden **Nimi**-kohdassa **Resurssienhallinta**-kohtaa hiiren kakkospainikkeella ja valitse sitten **Käynnistä uudelleen**.</span><span class="sxs-lookup"><span data-stu-id="116ef-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
