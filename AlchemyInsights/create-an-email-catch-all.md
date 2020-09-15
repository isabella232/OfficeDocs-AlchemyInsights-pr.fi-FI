---
title: Sähkö posti viestin luominen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712983"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="7786d-102">Sähkö posti viestin luominen</span><span class="sxs-lookup"><span data-stu-id="7786d-102">Create an email catch all</span></span>

<span data-ttu-id="7786d-103">Kaikkien saaliiden käyttöä ei suositella.</span><span class="sxs-lookup"><span data-stu-id="7786d-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="7786d-104">On parempi antaa lähettäjälle palautetta siitä, että lähettäjä saa viestin, että hänen viestinsä ei voitu toimittaa niin, että he voivat ryhtyä toimiin.</span><span class="sxs-lookup"><span data-stu-id="7786d-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="7786d-105">Voit myös rajoittaa valvotun posti laatikon koskemaan vain aiemmin kelvollisia Sähkö posti osoitteita.</span><span class="sxs-lookup"><span data-stu-id="7786d-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="7786d-106">Kaikki saalis kaikki posti laatikot saavat paljon roska postia ja saattavat lopulta täyttyä, jos ne eivät tarkkaan valvo.</span><span class="sxs-lookup"><span data-stu-id="7786d-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="7786d-107">(Saat rajoituksia.)</span><span class="sxs-lookup"><span data-stu-id="7786d-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="7786d-108">Jos päätät jatkaa, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="7786d-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="7786d-109">Luo dynaaminen jako ryhmä, & sisällyttää kaikki vastaanottajatyypit.</span><span class="sxs-lookup"><span data-stu-id="7786d-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="7786d-110">Luo oma posti laatikko sähkö postien pyytämisestä, esimerkiksi catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="7786d-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="7786d-111">Määritä tietylle toimi alueelle DomainType-asetukseksi "intern Relay".</span><span class="sxs-lookup"><span data-stu-id="7786d-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="7786d-112">Jos poistat kaikki saalis-asetukset myöhemmin, varmista, että toimi alue määritetään takaisin tärkeiksi.</span><span class="sxs-lookup"><span data-stu-id="7786d-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="7786d-113">Luo Mailflow-siirto sääntö seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="7786d-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="7786d-114">Jos lähettäjä on "organisaation ulkopuolinen"</span><span class="sxs-lookup"><span data-stu-id="7786d-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="7786d-115">Viestin uudelleenohjaus Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="7786d-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="7786d-116">Paitsi, jos edunsaaja on allusers@domain.com-jäsen (Distribution Group sisältää kaikki jäsenet)</span><span class="sxs-lookup"><span data-stu-id="7786d-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="7786d-117">Varmista, että uudet posti laatikot lisätään dynaamiseen jakeluun-ryhmään</span><span class="sxs-lookup"><span data-stu-id="7786d-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
