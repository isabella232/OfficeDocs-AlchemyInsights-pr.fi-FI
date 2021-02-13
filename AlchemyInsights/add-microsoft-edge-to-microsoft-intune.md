---
title: Microsoft Edgen lisääminen Microsoft Intuneen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194479"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="a4fd6-102">Microsoft Edgen lisääminen Microsoft Intuneen</span><span class="sxs-lookup"><span data-stu-id="a4fd6-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="a4fd6-103">Jotta voit ottaa Käyttöön, määrittää, valvoa ja suojata Microsoft Edge for Windows 10:tä, sinun on ensin lisättävä se Microsoft Intuneen.</span><span class="sxs-lookup"><span data-stu-id="a4fd6-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="a4fd6-104">Intune tukee Microsoft Edge 77:tä ja sitä uudempia versioita.</span><span class="sxs-lookup"><span data-stu-id="a4fd6-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="a4fd6-105">Intune havaitsee kaikki Microsoft Edgen aiemmat asennukset.</span><span class="sxs-lookup"><span data-stu-id="a4fd6-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="a4fd6-106">Jos Microsoft Edge asennetaan käyttäjäkontekstissa, järjestelmäasennus korvaa asennuksen käyttäjäkontekstissa.</span><span class="sxs-lookup"><span data-stu-id="a4fd6-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="a4fd6-107">Jos Microsoft Edge asennetaan järjestelmäkontekstissa, asennuksen onnistumisesta ilmoitetaan.</span><span class="sxs-lookup"><span data-stu-id="a4fd6-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="a4fd6-108">Esiasennettu Microsoft Edge 77 ja uudemmat versiot korvataan kaikissa käyttäjäkontekstin kanavilla, kun Microsoft Edge on asennettu järjestelmäkontekstiin.</span><span class="sxs-lookup"><span data-stu-id="a4fd6-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="a4fd6-109">**Edellytys**</span><span class="sxs-lookup"><span data-stu-id="a4fd6-109">**Prerequisite**</span></span>

<span data-ttu-id="a4fd6-110">Windows 10:n versio 1709 tai uudempi versio</span><span class="sxs-lookup"><span data-stu-id="a4fd6-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="a4fd6-111">**Vaiheet Edgen lisääminen Intuneen**</span><span class="sxs-lookup"><span data-stu-id="a4fd6-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="a4fd6-112">[Sovelluksen määrittäminen Intunessa.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="a4fd6-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="a4fd6-113">[Määritä sovelluksen tiedot.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="a4fd6-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="a4fd6-114">[Määritä sovelluksen asetukset.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="a4fd6-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="a4fd6-115">[Valitse vaikutusalueen tunnisteet (valinnainen).](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="a4fd6-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="a4fd6-116">[Lisää sovellus.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="a4fd6-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="a4fd6-117">Lisätietoja on ohjeaiheessa [Vianmääritys.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="a4fd6-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




