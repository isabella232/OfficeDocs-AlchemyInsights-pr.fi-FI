---
title: Muiden kuin Windows-laitteiden käytöstä poistaminen Microsoft Defender Advanced Threat Protectionista (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693812"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="6e810-102">Muiden kuin Windows-laitteiden käytöstä poistaminen Microsoft Defender Advanced Threat Protectionista (ATP)</span><span class="sxs-lookup"><span data-stu-id="6e810-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="6e810-103">Toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="6e810-103">Here's how:</span></span>

1. <span data-ttu-id="6e810-104">Jos haluat katkaista kolmannen osapuolen ratkaisun Microsoft Defender ATP:stä, noudata kolmannen osapuolen ohjeita.</span><span class="sxs-lookup"><span data-stu-id="6e810-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="6e810-105">Poista kolmannen osapuolen ratkaisun käyttöoikeudet Azure Active Directory -vuokraajassa:</span><span class="sxs-lookup"><span data-stu-id="6e810-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="6e810-106">Kirjaudu Sisään [Azure-portaaliin.](https://go.microsoft.com/fwlink/?linkid=2125612)</span><span class="sxs-lookup"><span data-stu-id="6e810-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="6e810-107">Valitse **Kaikki palvelut** Azure Active  >  **Directory** Enterprise  >  **Applications**.</span><span class="sxs-lookup"><span data-stu-id="6e810-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="6e810-108">Valitse sovellus, jonka haluat poistaa käytöstä.</span><span class="sxs-lookup"><span data-stu-id="6e810-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="6e810-109">Valitse **Poista.**</span><span class="sxs-lookup"><span data-stu-id="6e810-109">Select **Delete**.</span></span>

<span data-ttu-id="6e810-110">Lisätietoja on muiden kuin [Windows-laitteiden offboard-ohjeissa.](https://go.microsoft.com/fwlink/?linkid=2143630)</span><span class="sxs-lookup"><span data-stu-id="6e810-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
