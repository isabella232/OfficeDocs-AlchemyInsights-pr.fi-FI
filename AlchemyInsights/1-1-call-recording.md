---
title: Puhelun tallentaminen 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696919"
---
# <a name="11-call-recording"></a><span data-ttu-id="dc193-102">Puhelun tallentaminen 1:1</span><span class="sxs-lookup"><span data-stu-id="dc193-102">1:1 call recording</span></span>

<span data-ttu-id="dc193-103">Jos Aloita **tallennus -painike** näkyy harmaana yhden puhelun aikana, sinun on muutettava käyttäjän käytäntöasetuksia.</span><span class="sxs-lookup"><span data-stu-id="dc193-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="dc193-104">31. toukokuuta 2021 alkaen otamme käyttöön uuden puhelukäytännön *AllowCloudRecordingForCalls Teams* käyttöön.</span><span class="sxs-lookup"><span data-stu-id="dc193-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="dc193-105">Ennen tätä muutosta 1:1-puhelutallenteen hallinnassa on *AllowCloudRecording* Teams kokouskäytäntö.</span><span class="sxs-lookup"><span data-stu-id="dc193-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="dc193-106">Tämä muutos on dokumentoitu viestikeskuksen viestissä: [(Päivitetty) 1:1 Puhelutallennuskäytännön esittely](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span><span class="sxs-lookup"><span data-stu-id="dc193-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="dc193-107">*AllowCloudRecordingForCalls*   puhelukäytäntöasetus on **$False** oletusarvoisesti.</span><span class="sxs-lookup"><span data-stu-id="dc193-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="dc193-108">Jos haluat estää kaikkia käyttäjiä nauhoittamaan 1:1-puheluita, sinun ei tarvitse tehdä mitään.</span><span class="sxs-lookup"><span data-stu-id="dc193-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="dc193-109">Jos haluat ottaa puhelutallenteen käyttöön kaikille käyttäjille 1:1-puheluissa, suorita Teams cmdlet-komento PowerShellin avulla:</span><span class="sxs-lookup"><span data-stu-id="dc193-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="dc193-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="dc193-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="dc193-111">Vaihtoehtoisesti voit luoda uuden käytännön ja määrittää **AllowCloudRecordingForCalls** -$true **ja** määrittää käytännön käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="dc193-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="dc193-112">Lisätietoja on kohdassa [1:1 Puhelun tallennuskäytännön ohjausobjektit ovat (lähes!) Täällä](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="dc193-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
