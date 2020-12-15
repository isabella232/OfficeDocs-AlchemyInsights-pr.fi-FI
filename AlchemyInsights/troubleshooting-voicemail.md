---
title: 'Vasta ajan vian määritys '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677962"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="aad51-102">Vasta ajan vian määritys</span><span class="sxs-lookup"><span data-stu-id="aad51-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="aad51-103">Varmista, että varattu varattu-ominaisuus on tarkoituksellinen.</span><span class="sxs-lookup"><span data-stu-id="aad51-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="aad51-104">Jos tätä ominaisuutta ei tarvita tällä käyttäjällä:</span><span class="sxs-lookup"><span data-stu-id="aad51-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="aad51-105">Siirry [teamsin hallinta keskukseen](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="aad51-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="aad51-106">Valitse vasemman reunan ääni puhelun   >  **käytännöt**-kohdan  >  **puhelu käytännön\*\*\*\*käytäntöjen hallinta** .</span><span class="sxs-lookup"><span data-stu-id="aad51-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="aad51-107">Valitse **Hallitse käyttäjiä**.</span><span class="sxs-lookup"><span data-stu-id="aad51-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="aad51-108">Hae käyttäjää ja muuta puhelu käytäntöä, joka on varattu varattu-asetuksena on käytössä, **Kun puhelu** on **poissa käytöstä**.</span><span class="sxs-lookup"><span data-stu-id="aad51-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="aad51-109">Valitse **Käytä**.</span><span class="sxs-lookup"><span data-stu-id="aad51-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="aad51-110">Käytäntöjen muutokset voivat kestää jopa 24 tuntia, ennen kuin ne replikoidaan.</span><span class="sxs-lookup"><span data-stu-id="aad51-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="aad51-111">Lisä tietoja tästä ominaisuudesta on kohdassa: varattu on varattu-toiminto [on käytettävissä puhelun aikana](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="aad51-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
