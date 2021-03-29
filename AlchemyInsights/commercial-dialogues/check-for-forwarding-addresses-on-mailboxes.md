---
title: Postilaatikoiden edelleenlähetysosoitteiden etsiminen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403308"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="a1eef-102">Postilaatikoiden edelleenlähetysosoitteiden etsiminen</span><span class="sxs-lookup"><span data-stu-id="a1eef-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="a1eef-103">Joskus hakkerit välittämään käyttäjien sähköpostiviestit itselleen, joten tarkistamme ensin postilaatikon edelleenlähetysosoitteet ja -säännöt.</span><span class="sxs-lookup"><span data-stu-id="a1eef-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="a1eef-104">Tarkistamme sitten valvontalokit.</span><span class="sxs-lookup"><span data-stu-id="a1eef-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="a1eef-105">Voit tarkistaa osoitteiden edelleenlähetysosoitteet näin:</span><span class="sxs-lookup"><span data-stu-id="a1eef-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="a1eef-106">Valitse   >  **Käyttäjät, jotka ovat aktiivisia käyttäjiä.**</span><span class="sxs-lookup"><span data-stu-id="a1eef-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="a1eef-107">Valitse käyttäjä, jonka tiliä on käytetty.</span><span class="sxs-lookup"><span data-stu-id="a1eef-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="a1eef-108">Laajenna esiin tulevassa pikaikkunassa **Postiasetukset** ja valitse sitten **Muokkaa** sähköpostin **edelleenlähetystä varten.**</span><span class="sxs-lookup"><span data-stu-id="a1eef-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="a1eef-109">Poista edelleenlähetysosoitteet, jotka et tunnista.</span><span class="sxs-lookup"><span data-stu-id="a1eef-109">Remove any forwarding addresses you don't recognize.</span></span>