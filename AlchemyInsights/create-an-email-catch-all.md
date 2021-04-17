---
title: Sähköpostiviestin luominen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816197"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="15cae-102">Sähköpostiviestin luominen</span><span class="sxs-lookup"><span data-stu-id="15cae-102">Create an email catch all</span></span>

<span data-ttu-id="15cae-103">Kaikkien takuiden käyttö ei ole suositeltavaa.</span><span class="sxs-lookup"><span data-stu-id="15cae-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="15cae-104">On parempi antaa lähettäjälle ilmoitus viestin lähettäjälle siitä, että viestiä ei voitu toimittaa osoitettaan, jotta lähettäjä voi ryhtyä toimenpiteisiin.</span><span class="sxs-lookup"><span data-stu-id="15cae-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="15cae-105">Voit myös rajoittaa valvotulle postilaatikolle vain aiemmin kelvolliset sähköpostiosoitteet.</span><span class="sxs-lookup"><span data-stu-id="15cae-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="15cae-106">Kaikki kaikki postilaatikot saavat paljon roskapostia, ja ne saattavat täyty, jos niitä ei valvota tarkasti.</span><span class="sxs-lookup"><span data-stu-id="15cae-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="15cae-107">(Rajoituksia on.)</span><span class="sxs-lookup"><span data-stu-id="15cae-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="15cae-108">Jos haluat jatkaa, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="15cae-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="15cae-109">Luo dynaaminen jakeluryhmä, & "Kaikki vastaanottajatyypit".</span><span class="sxs-lookup"><span data-stu-id="15cae-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="15cae-110">Luo erillinen postilaatikko sähköpostiviestien pyytä varten, esimerkiksi catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="15cae-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="15cae-111">Määritä tietyn toimialueen DomainType-tyypiksi InternalRelay.</span><span class="sxs-lookup"><span data-stu-id="15cae-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="15cae-112">Jos poistat kaikki toimialueet myöhemmin, muista määrittää toimialue takaisin arvoksi Authoritative.</span><span class="sxs-lookup"><span data-stu-id="15cae-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="15cae-113">Luo Postinkulku-siirtosääntö seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="15cae-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="15cae-114">Jos lähettäjä on Organisaation ulkopuolinen</span><span class="sxs-lookup"><span data-stu-id="15cae-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="15cae-115">Ohjaa viesti Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="15cae-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="15cae-116">Paitsi jos vastaanottaja on jäsen allusers@domain.com (Jakeluryhmä sisältää kaikki jäsenet)</span><span class="sxs-lookup"><span data-stu-id="15cae-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="15cae-117">Varmista, että uudet postilaatikot lisätään dynaamiseen jakeluryhmään</span><span class="sxs-lookup"><span data-stu-id="15cae-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
