---
title: Applen automaattisen laite rekisteröinnin synkronointi virheet
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714736"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="2344e-102">Applen automaattisen laite rekisteröinnin synkronointi virheet</span><span class="sxs-lookup"><span data-stu-id="2344e-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="2344e-103">"Olemme havainneet, että sinulla on yksi tai useampia ADE/DEP-tunnuksia, jotka ovat virhe tilassa.</span><span class="sxs-lookup"><span data-stu-id="2344e-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="2344e-104">Jos virhe tila on ratkennut kunkin heikkouden sisältävän tunnus sanoman kohdalla, ADE-toiminnallisuus ei toimi samalla tavalla.</span><span class="sxs-lookup"><span data-stu-id="2344e-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="2344e-105">Tämä virhe voi ilmetä useilla eri tavoilla, kuten:</span><span class="sxs-lookup"><span data-stu-id="2344e-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="2344e-106">Laitteet eivät voi synkronoitua ABM/ass:ssä Intuneen</span><span class="sxs-lookup"><span data-stu-id="2344e-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="2344e-107">Rekisteröinti profiilin määritykset voivat epäonnistua</span><span class="sxs-lookup"><span data-stu-id="2344e-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="2344e-108">Laitteet eivät välttämättä ole täydellisiä ADE-rekisteröinnin onnistumisen</span><span class="sxs-lookup"><span data-stu-id="2344e-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="2344e-109">Tarkista, onko Intune-konsolissa ilmoitettu synkronointi virhe kohdassa **laitteet > rekisteröi laitteet > Apple-rekisteröinti > rekisteröinti ohjelman tunnukset** ja tarkastele mahdollisia korjaus toimenpiteitä seuraavien ohjeiden mukaisesti:</span><span class="sxs-lookup"><span data-stu-id="2344e-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="2344e-110">ABM-ja Ibios-synkronointi virheet iOS/iPadOS-ja macOS-automatisoitujen laitteiden rekisteröinti tunnukset</span><span class="sxs-lookup"><span data-stu-id="2344e-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
