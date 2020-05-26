---
title: Tarvitsetko apua sähköpostin lähetysrajoitusten kanssa?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357547"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="c9040-102">Tarvitsetko apua sähköpostin lähetysrajoitusten kanssa?</span><span class="sxs-lookup"><span data-stu-id="c9040-102">Need help with email sending limits?</span></span>

<span data-ttu-id="c9040-103">Alla on **käytössä mallikohtaiset lähetysrajat,** jotka on pantu täytäntöön palvelussa.</span><span class="sxs-lookup"><span data-stu-id="c9040-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="c9040-104">Lisätietoja näistä rajoituksista on dokumentoitu [tässä](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="c9040-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="c9040-105">Ei-toivottujen joukkoviestien toimittamisen estämiseksi käytämme **käyttäjäkohtaisia vastaanottajien hintarajoituksia kaikkiin lähteviin ja sisäisiin viesteihin.**</span><span class="sxs-lookup"><span data-stu-id="c9040-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="c9040-106">Kaikissa varastointiyksiköissä tämä raja on **10 000 vastaanottajaa päivässä.**</span><span class="sxs-lookup"><span data-stu-id="c9040-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="c9040-107">Asiakkaiden, joiden on lähetettävä laillinen joukkokaupallinen sähköposti (esimerkiksi asiakastiedotteet), tulee käyttää näihin palveluihin erikoistuneita kolmannen osapuolen palveluntarjoajia.</span><span class="sxs-lookup"><span data-stu-id="c9040-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="c9040-108">**Huomautus**: Kun vastaanottajan nopeusrajoitus on saavutettu, viestejä ei voi lähettää postilaatikosta, ennen kuin viimeisten 24 tunnin aikana lähetettyjen vastaanottajien määrä laskee rajan alapuolelle.</span><span class="sxs-lookup"><span data-stu-id="c9040-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="c9040-109">Käyttäjä ei voi lähettää viestejä ennen tätä kohtaa.</span><span class="sxs-lookup"><span data-stu-id="c9040-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="c9040-110">Viestien nopeusrajoitus **on 30 viestiä minuutissa** kaikissa varastointiyksiköissä.</span><span class="sxs-lookup"><span data-stu-id="c9040-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="c9040-111">Tämä määrittää, kuinka monta viestiä käyttäjä voi lähettää Exchange Online -tililtään tietyn ajan kuluessa.</span><span class="sxs-lookup"><span data-stu-id="c9040-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="c9040-112">Yksittäisen **sähköpostiviestin Vastaanottaja-, Kopio- ja Piilokopio-kentissä sallittujen vastaanottajien enimmäismäärä** kaikissa varastointiyksiköissä on **1 000 vastaanottajaa.**</span><span class="sxs-lookup"><span data-stu-id="c9040-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="c9040-113">Voit mukauttaa tätä rajaa [siirtymällä tähän](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="c9040-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
