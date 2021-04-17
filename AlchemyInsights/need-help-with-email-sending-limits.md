---
title: Tarvitsetko apua sähköpostin lähetysrajoitusten kanssa?
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
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836276"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="939f2-102">Tarvitsetko apua sähköpostin lähetysrajoitusten kanssa?</span><span class="sxs-lookup"><span data-stu-id="939f2-102">Need help with email sending limits?</span></span>

<span data-ttu-id="939f2-103">Alla on palvelussa käytössä olevat **suunnitellut lähetysrahat**.</span><span class="sxs-lookup"><span data-stu-id="939f2-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="939f2-104">Lisätietoja rajoituksista on [täällä](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="939f2-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="939f2-105">Jotta ei-toivottujen joukkoviestien toimittamista voidaan estää, on sovellettava käyttäjäkohtaisia **kaikkien lähtevien ja sisäisten viestien vastaanottajien tiedonsiirtorajoituksia**.</span><span class="sxs-lookup"><span data-stu-id="939f2-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="939f2-106">Tämä rajoitus on kaikissa SKU:issa **10 000 vastaanottajaa päivässä**.</span><span class="sxs-lookup"><span data-stu-id="939f2-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="939f2-107">Asiakkaiden, joiden on lähetettävä laillisia kaupallisia joukkosähköposteja (esimerkiksi asiakastiedotteet), on käytettävä näihin palveluihin kolmannen osapuolen tarjoajia, jotka ovat erikoistuneet niihin.</span><span class="sxs-lookup"><span data-stu-id="939f2-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="939f2-108">**Huomautus**: Kun vastaanottajan tiedonsiirtorajoitus on saavutettu, viestejä ei voi lähettää postilaatikosta ennen kuin viimeisten 24 tunnin aikana lähetettyjen viestien vastaanottajien määrä laskee alle sallitun määrän.</span><span class="sxs-lookup"><span data-stu-id="939f2-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="939f2-109">Käyttäjä ei voi lähettää viestejä ennen tätä.</span><span class="sxs-lookup"><span data-stu-id="939f2-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="939f2-110">Viestirajaa **30 viestiä minuutissa** käytetään kaikissa SKU:issa.</span><span class="sxs-lookup"><span data-stu-id="939f2-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="939f2-111">Tämä määrittää sen, kuinka monta viestiä käyttäjä voi lähettää Exchange Online -tilinsä kautta tietyn ajanjakson aikana.</span><span class="sxs-lookup"><span data-stu-id="939f2-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="939f2-112">**Vastaanottaja-, kopio- ja piilokopio** kentissä sallittujen vastaanottajien enimmäismäärä on kaikissa SKU:issa yhdelle viestille **1 000 vastaanottajaa**.</span><span class="sxs-lookup"><span data-stu-id="939f2-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="939f2-113">Voit mukauttaa tätä rajoitusta [täällä](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="939f2-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
