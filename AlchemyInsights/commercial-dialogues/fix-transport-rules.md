---
title: Siirtosääntöjen ratkaiseminen
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746739"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="a43ee-102">Siirtosääntöjen ratkaiseminen</span><span class="sxs-lookup"><span data-stu-id="a43ee-102">Fix transport rules</span></span>

<span data-ttu-id="a43ee-103">Tämä sanoma vaikuttaa mukautettuun postinkulkusääntöön.</span><span class="sxs-lookup"><span data-stu-id="a43ee-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="a43ee-104">Voit tarkistaa täsmällisen säännön seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="a43ee-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="a43ee-105">Huomaa lähetyksen tuloksissa **Lisätietoja-kohdassa** **GUID-tunnus** tai **käytännön nimi.**</span><span class="sxs-lookup"><span data-stu-id="a43ee-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="a43ee-106">Käynnistä Exchange-hallintaliittymä.</span><span class="sxs-lookup"><span data-stu-id="a43ee-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="a43ee-107">Lisätietoja on ohjeaiheessa [Exchange-hallintaliittymän avaaminen.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="a43ee-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="a43ee-108">Suorita tämä komento (käyttämällä lähetyksen  **GUID-tunnusta): Get-TransportRule -identity "GUID" | fl \* Description**\*</span><span class="sxs-lookup"><span data-stu-id="a43ee-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="a43ee-109">Tarkista kuvaus, jotta näet määritetyt ehdot, joihin viesti vaikuttaa.</span><span class="sxs-lookup"><span data-stu-id="a43ee-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="a43ee-110">Lisätietoja on kohdassa [Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)</span><span class="sxs-lookup"><span data-stu-id="a43ee-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
