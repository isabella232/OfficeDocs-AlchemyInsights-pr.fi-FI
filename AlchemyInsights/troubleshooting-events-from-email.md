---
title: Sähköpostitapahtumien vianmääritys
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834836"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="2a216-102">Sähköpostitapahtumien vianmääritys</span><span class="sxs-lookup"><span data-stu-id="2a216-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="2a216-103">Tarkista, että ominaisuus on otettu käyttöön postilaatikossa: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="2a216-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="2a216-104">Katso sitten Tapahtumat sähköpostista -lokeja **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="2a216-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="2a216-105">Etsi Tapahtumat sähköpostista -lokeihin InternetMessageId, joka vastaa postilaatikon kohdetta.</span><span class="sxs-lookup"><span data-stu-id="2a216-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="2a216-106">TrustScore määrittää, lisätäänkö kohde vai ei.</span><span class="sxs-lookup"><span data-stu-id="2a216-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="2a216-107">Tapahtumat lisätään vain, jos TrustScore = "Luotettu".</span><span class="sxs-lookup"><span data-stu-id="2a216-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="2a216-108">TrustScore määritetään SPF-, Dkim- tai Dmarc-ominaisuuksien mukaan, jotka ovat viestin otsikossa.</span><span class="sxs-lookup"><span data-stu-id="2a216-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="2a216-109">Voit tarkastella näitä ominaisuuksia seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="2a216-109">To view these properties:</span></span>

<span data-ttu-id="2a216-110">**Outlookin työpöytäversio**</span><span class="sxs-lookup"><span data-stu-id="2a216-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="2a216-111">Avaa kohde</span><span class="sxs-lookup"><span data-stu-id="2a216-111">Open the item</span></span>
- <span data-ttu-id="2a216-112">Tiedosto -> -> Internet-otsikot</span><span class="sxs-lookup"><span data-stu-id="2a216-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="2a216-113">TAI</span><span class="sxs-lookup"><span data-stu-id="2a216-113">or</span></span>

<span data-ttu-id="2a216-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="2a216-114">**MFCMapi**</span></span>

- <span data-ttu-id="2a216-115">Siirtyminen Saapuneet-kansion kohteeseen</span><span class="sxs-lookup"><span data-stu-id="2a216-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="2a216-116">Etsi PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="2a216-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="2a216-117">Nämä ominaisuudet määritetään ja tallennetaan reitityksen ja reitityksen aikana.</span><span class="sxs-lookup"><span data-stu-id="2a216-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="2a216-118">Jos tarvitset lisää vianmääritystä, sinun on ehkä seurattava siirtotukea SPF-, DKIM- ja DMARC-virheistä.</span><span class="sxs-lookup"><span data-stu-id="2a216-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>