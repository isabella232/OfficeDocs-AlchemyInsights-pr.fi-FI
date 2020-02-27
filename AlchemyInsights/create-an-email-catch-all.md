---
title: Luo sähköposti saalis kaikki
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286107"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="40501-102">Luo sähköposti saalis kaikki</span><span class="sxs-lookup"><span data-stu-id="40501-102">Create an email catch all</span></span>

<span data-ttu-id="40501-103">Saaliin käyttö kaikki on erittäin suositeltavaa.</span><span class="sxs-lookup"><span data-stu-id="40501-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="40501-104">On parempi antaa kimpsää lähettäjälle, jotta lähettäjät tietävät, että heidän viestiäei voitu toimittaa, jotta he voivat toimia.</span><span class="sxs-lookup"><span data-stu-id="40501-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="40501-105">Voit myös rajoittaa valvotun postilaatikon vain kiinni aiemmin kelvollisia sähköpostiosoitteita.</span><span class="sxs-lookup"><span data-stu-id="40501-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="40501-106">Kaikki saalis kaikki postilaatikko saa paljon roskapostia ja voi lopulta täyttää, jos ei tarkasti seurattava.</span><span class="sxs-lookup"><span data-stu-id="40501-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="40501-107">(Raja-arvoja vastaanotetaan.)</span><span class="sxs-lookup"><span data-stu-id="40501-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="40501-108">Jos päätät jatkaa, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="40501-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="40501-109">Luo dynaaminen jakeluryhmä, & sisältää "Kaikki vastaanottajatyypit".</span><span class="sxs-lookup"><span data-stu-id="40501-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="40501-110">Luo oma postilaatikko, jossa voit esimerkiksi catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="40501-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="40501-111">Määritä tietylle toimialueelle DomainType-arvoksi InternalRelay.</span><span class="sxs-lookup"><span data-stu-id="40501-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="40501-112">Jos poistat saaliin myöhemmin, muista asettaa toimialueen takaisin arvovaltaiseksi.</span><span class="sxs-lookup"><span data-stu-id="40501-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="40501-113">Luo postivulähetyksen kuljetussääntö seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="40501-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="40501-114">Jos lähettäjä on "Organisaation ulkopuolella"</span><span class="sxs-lookup"><span data-stu-id="40501-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="40501-115">Ohjaa viesti uudelleen Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="40501-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="40501-116">Paitsi jos vastaanottaja on allusers@domain.com jäsen (jakeluryhmä sisältää kaikki jäsenet)</span><span class="sxs-lookup"><span data-stu-id="40501-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="40501-117">Varmista, että dynaamiseen jakeluryhmään lisätään uusia postilaatikoita</span><span class="sxs-lookup"><span data-stu-id="40501-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
