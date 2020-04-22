---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707908"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="3da69-102">Korjaa virhekoodin 550 5.4.1 välityskäytön ongelmat estetty</span><span class="sxs-lookup"><span data-stu-id="3da69-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="3da69-103">Tämä ongelma [ilmenee, kun tarkistetaan, onko sähköpostiosoite kelvollinen estämään palautus,](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) kun siirryt Microsoft-verkkoon.</span><span class="sxs-lookup"><span data-stu-id="3da69-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="3da69-104">Kokeile seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="3da69-104">Try the following:</span></span>

1. <span data-ttu-id="3da69-105">Selvitä, liittyykö ongelma koko toimialueeseen vai yhteen sähköpostiosoitteeseen:</span><span class="sxs-lookup"><span data-stu-id="3da69-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="3da69-106">Koko toimialue: Joskus toimialue on synkronoitava; yritä [asettaa toimialue sisäiseksi ja sitten takaisin arvovaltaiseen](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="3da69-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="3da69-107">Yksittäinen sähköpostiosoite: Joskus osoite on synkronoitava; ailahteleminen smtp valtuutettu edustaja kohdistaa ja niin muodoin ailahteleminen se taaksepäin kanisteri auttaa.</span><span class="sxs-lookup"><span data-stu-id="3da69-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="3da69-108">Selvitä, liittyykö ongelma ryhmään vai yleiseen kansioon.</span><span class="sxs-lookup"><span data-stu-id="3da69-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="3da69-109">Joissakin objektityypeissä objektit on ehkä luotava manuaalisesti Azure Active Directoryssa.</span><span class="sxs-lookup"><span data-stu-id="3da69-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="3da69-110">Jos tarvitset lisäapua, avaa tukipyyntö ja määritä ongelman laajuus (mukaan lukien lähetettävän objektin tyyppi), jotta voimme auttaa sinua paremmin.</span><span class="sxs-lookup"><span data-stu-id="3da69-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>