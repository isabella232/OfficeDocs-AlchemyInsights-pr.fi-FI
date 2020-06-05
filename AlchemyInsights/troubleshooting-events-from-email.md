---
title: Tapahtumien vianmääritys sähköpostista
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569143"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="bc841-102">Tapahtumien vianmääritys sähköpostista</span><span class="sxs-lookup"><span data-stu-id="bc841-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="bc841-103">Varmista, että ominaisuus on otettu käyttöön postilaatikossa: \*\*Get-EventsFromEmailConfiguration -Identity <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="bc841-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="bc841-104">Katso sitten "Tapahtumat sähköpostista" lokit **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="bc841-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="bc841-105">Etsi Sähköpostitapahtumat-lokit -lokista internetmessageId, joka vastaa postilaatikon kohdetta.</span><span class="sxs-lookup"><span data-stu-id="bc841-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="bc841-106">TrustScore määrittää, lisätäänkö kohde vai ei.</span><span class="sxs-lookup"><span data-stu-id="bc841-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="bc841-107">Tapahtumat lisätään vain, jos TrustScore = "Luotettu".</span><span class="sxs-lookup"><span data-stu-id="bc841-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="bc841-108">TrustScore määräytyy SPF-, Dkim- tai Dmarc-ominaisuuksien mukaan, jotka ovat viestin otsikossa.</span><span class="sxs-lookup"><span data-stu-id="bc841-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="bc841-109">Voit tarkastella näitä ominaisuuksia seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="bc841-109">To view these properties:</span></span>

<span data-ttu-id="bc841-110">**Työpöydän Outlook**</span><span class="sxs-lookup"><span data-stu-id="bc841-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="bc841-111">Kohteen avaaminen</span><span class="sxs-lookup"><span data-stu-id="bc841-111">Open the item</span></span>
- <span data-ttu-id="bc841-112">Tiedosto -> Ominaisuudet -> Internet-otsikot</span><span class="sxs-lookup"><span data-stu-id="bc841-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="bc841-113">TAI</span><span class="sxs-lookup"><span data-stu-id="bc841-113">or</span></span>

<span data-ttu-id="bc841-114">**Kävi koulua MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="bc841-114">**MFCMapi**</span></span>

- <span data-ttu-id="bc841-115">Siirry Saapuneet-kansion kohteeseen</span><span class="sxs-lookup"><span data-stu-id="bc841-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="bc841-116">Etsi PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="bc841-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="bc841-117">Nämä ominaisuudet määritetään ja tallennetaan kuljetuksen ja reitityksen aikana.</span><span class="sxs-lookup"><span data-stu-id="bc841-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="bc841-118">Lisävianmääritystä varten sinun on ehkä seurattava Kuljetustukea SPF:n, DKIM:n ja DMARC:n epäonnistumisista.</span><span class="sxs-lookup"><span data-stu-id="bc841-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>