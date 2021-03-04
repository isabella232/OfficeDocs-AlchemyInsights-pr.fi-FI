---
title: Postilaatikoiden edelleenlähetysosoitteiden etsiminen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427329"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="1ec52-102">Postilaatikoiden edelleenlähetysosoitteiden etsiminen</span><span class="sxs-lookup"><span data-stu-id="1ec52-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="1ec52-103">Joskus hakkerit välittämään käyttäjien sähköpostiviestit itselleen, joten tarkistamme ensin postilaatikon edelleenlähetysosoitteet ja -säännöt.</span><span class="sxs-lookup"><span data-stu-id="1ec52-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="1ec52-104">Tarkistamme sitten valvontalokit.</span><span class="sxs-lookup"><span data-stu-id="1ec52-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="1ec52-105">Voit tarkistaa osoitteiden edelleenlähetysosoitteet näin:</span><span class="sxs-lookup"><span data-stu-id="1ec52-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="1ec52-106">Valitse   >  **Käyttäjät, jotka ovat aktiivisia käyttäjiä.**</span><span class="sxs-lookup"><span data-stu-id="1ec52-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="1ec52-107">Valitse käyttäjä, jonka tiliä on käytetty.</span><span class="sxs-lookup"><span data-stu-id="1ec52-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="1ec52-108">Laajenna esiin tulevassa pikaikkunassa **Postiasetukset** ja valitse sitten Muokkaa **sähköpostin** **edelleenlähetystä varten.**</span><span class="sxs-lookup"><span data-stu-id="1ec52-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="1ec52-109">Poista edelleenlähetysosoitteet, jotka et tunnista.</span><span class="sxs-lookup"><span data-stu-id="1ec52-109">Remove any forwarding addresses you don't recognize.</span></span>