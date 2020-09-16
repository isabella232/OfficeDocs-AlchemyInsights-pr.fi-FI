---
title: Tapahtumien vian määritys sähkö postista
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658731"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="d7c4b-102">Tapahtumien vian määritys sähkö postista</span><span class="sxs-lookup"><span data-stu-id="d7c4b-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="d7c4b-103">Tarkista, että ominaisuus on otettu käyttöön posti laatikolle: **Get-EventsFromEmailConfiguration <mailbox> -Identity**</span><span class="sxs-lookup"><span data-stu-id="d7c4b-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="d7c4b-104">Katso sitten tapahtumat sähkö postista-lokit **vienti-Mailposti-Diagnosticlogs <mailbox> -Component timeprofile**</span><span class="sxs-lookup"><span data-stu-id="d7c4b-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="d7c4b-105">Etsi tapahtumat Sähkö posti-lokista-kohdassa InternetMessageId, joka vastaa posti laatikon kohdetta.</span><span class="sxs-lookup"><span data-stu-id="d7c4b-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="d7c4b-106">TrustScore määrittää, lisätäänkö kohde vai ei.</span><span class="sxs-lookup"><span data-stu-id="d7c4b-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="d7c4b-107">Tapahtumia lisätään vain, jos Trustiscore = "luotettu".</span><span class="sxs-lookup"><span data-stu-id="d7c4b-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="d7c4b-108">TrustScore määräytyy SPF-, DKIM-tai dMarc-ominaisuuksien mukaan, jotka ovat viestin otsikossa.</span><span class="sxs-lookup"><span data-stu-id="d7c4b-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="d7c4b-109">Voit tarkastella näitä ominaisuuksia seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="d7c4b-109">To view these properties:</span></span>

<span data-ttu-id="d7c4b-110">**Desktop Outlook**</span><span class="sxs-lookup"><span data-stu-id="d7c4b-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="d7c4b-111">Kohteen avaaminen</span><span class="sxs-lookup"><span data-stu-id="d7c4b-111">Open the item</span></span>
- <span data-ttu-id="d7c4b-112">Tiedosto-> ominaisuudet-> Internet-otsikot</span><span class="sxs-lookup"><span data-stu-id="d7c4b-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="d7c4b-113">TAI</span><span class="sxs-lookup"><span data-stu-id="d7c4b-113">or</span></span>

<span data-ttu-id="d7c4b-114">**Mfcmapia**</span><span class="sxs-lookup"><span data-stu-id="d7c4b-114">**MFCMapi**</span></span>

- <span data-ttu-id="d7c4b-115">Saapuneet-kansiossa olevaan kohteeseen siirtyminen</span><span class="sxs-lookup"><span data-stu-id="d7c4b-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="d7c4b-116">Etsi PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="d7c4b-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="d7c4b-117">Nämä ominaisuudet määritetään ja tallennetaan kuljetuksen ja reitityksen aikana.</span><span class="sxs-lookup"><span data-stu-id="d7c4b-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="d7c4b-118">Jos haluat lisä tietoja vian määrityksestä, sinun on ehkä seurattava siirto tukea SPF-, DKIM-ja.-tai DMARC-virheiden varalta.</span><span class="sxs-lookup"><span data-stu-id="d7c4b-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>