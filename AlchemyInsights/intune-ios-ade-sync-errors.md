---
title: Applen automaattisen laitteen rekisteröinnin synkronointivirheet
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448919"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="8e53f-102">Applen automaattisen laitteen rekisteröinnin synkronointivirheet</span><span class="sxs-lookup"><span data-stu-id="8e53f-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="8e53f-103">"Olemme havainneet, että sinulla on yksi tai useampi ADE/DEP-tunnus, joka on virhetilassa.</span><span class="sxs-lookup"><span data-stu-id="8e53f-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="8e53f-104">Ennen kuin virhetila on ratkaistu kunkin tunnuksen osalta, ADE-toiminto ei toimi odotetulla tavalla."</span><span class="sxs-lookup"><span data-stu-id="8e53f-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="8e53f-105">Tämä virhe voi ilmetä monin eri tavoin, kuten:</span><span class="sxs-lookup"><span data-stu-id="8e53f-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="8e53f-106">Laitteet eivät ehkä synkronoidu ABM/ASM:stä Intuneen</span><span class="sxs-lookup"><span data-stu-id="8e53f-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="8e53f-107">Rekisteröintiprofiilimääritykset saattavat epäonnistua</span><span class="sxs-lookup"><span data-stu-id="8e53f-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="8e53f-108">Laitteet eivät ehkä suorita ADE-rekisteröintiä onnistuneesti</span><span class="sxs-lookup"><span data-stu-id="8e53f-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="8e53f-109">Tarkista Intune-konsolissa ilmoitettu synkronointivirhe Laitteet-kohdassa, > rekisteröi laitteet **> Apple-rekisteröinti>-ohjelman tunnukset.**</span><span class="sxs-lookup"><span data-stu-id="8e53f-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="8e53f-110">Yksi yleisimmistä synkronointivirheen syistä on nykyisen tunnuksen vanheneminen.</span><span class="sxs-lookup"><span data-stu-id="8e53f-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="8e53f-111">Monissa tapauksissa ongelma ratkeaa, jos kyseinen tunnus uusitaan.</span><span class="sxs-lookup"><span data-stu-id="8e53f-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="8e53f-112">Jos vähintään yksi tunnuksesi on vanhentunut, tutustu seuraaviin ohjeisiin, joiden avulla voit uusia ne tarpeen mukaan:</span><span class="sxs-lookup"><span data-stu-id="8e53f-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="8e53f-113">Automaattisen laitteen rekisteröintitunnuksen uusiminen</span><span class="sxs-lookup"><span data-stu-id="8e53f-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="8e53f-114">Lisäksi seuraavista ohjeista näet mahdolliset korjaaminen muista virheistä, jotka aiheuttavat tunnusten synkronointivirheitä:</span><span class="sxs-lookup"><span data-stu-id="8e53f-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="8e53f-115">ABM-/ASM-synkronointivirheet iOS-/iPadOS- ja macOS-laitteiden automaattisen rekisteröinnin tunnuksille</span><span class="sxs-lookup"><span data-stu-id="8e53f-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="8e53f-116">ABM-/ASM-synkronointivirheet iOS-/iPadOS- ja macOS-laitteiden automaattisen rekisteröinnin tunnuksille</span><span class="sxs-lookup"><span data-stu-id="8e53f-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
