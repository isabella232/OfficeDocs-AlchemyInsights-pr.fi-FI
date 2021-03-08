---
title: Mukautetun toimialueen ottaminen käyttöön DKIM:ssä
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 1a21101602f47dcb5c9b607d7bbccfacec00f43a
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524125"
---
# <a name="enable-the-custom-domain-for-dkim"></a><span data-ttu-id="59f5d-102">Mukautetun toimialueen ottaminen käyttöön DKIM:ssä</span><span class="sxs-lookup"><span data-stu-id="59f5d-102">Enable the custom domain for DKIM</span></span>

<span data-ttu-id="59f5d-103">Kun olet luonut CNAME-tietueet mukautettuja toimialueita varten, sinun on otettava toimialue käyttöön.</span><span class="sxs-lookup"><span data-stu-id="59f5d-103">After you create the CNAME records for your custom domains, you need to enable the domain.</span></span>

<span data-ttu-id="59f5d-104">Voit ottaa toimialueen käyttöön seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="59f5d-104">To enable the domain, perform the following steps:</span></span>

1. <span data-ttu-id="59f5d-105">Siirry [Exchange-hallintakeskukseen.](https://outlook.office365.com/ecp/)</span><span class="sxs-lookup"><span data-stu-id="59f5d-105">Navigate to the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>
2. <span data-ttu-id="59f5d-106">Valitse vasemmanpuoleisessa **ruudussa > dkim.**</span><span class="sxs-lookup"><span data-stu-id="59f5d-106">In the left pane, select **protection > dkim**.</span></span>
3. <span data-ttu-id="59f5d-107">Valitse toimialue ja valitse sitten Allekirjoita tämän toimialueen **viestit DKIM-allekirjoituksella**-kohdassa **Ota käyttöön.**</span><span class="sxs-lookup"><span data-stu-id="59f5d-107">Select the domain, and then under **Sign messages for this domain with DKIM signatures**, click **Enable**.</span></span> <span data-ttu-id="59f5d-108">Toista tämä vaihe jokaiselle toimialueelle.</span><span class="sxs-lookup"><span data-stu-id="59f5d-108">Repeat this step for each domain.</span></span>

