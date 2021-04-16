---
title: Virhe SpamHausin estämiä sähköpostiviestejä lähetettäessä
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813721"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="2d5de-102">Virhe sähköpostin lähettämisessä: Asiakkaan isäntä estetty Spamhausin avulla</span><span class="sxs-lookup"><span data-stu-id="2d5de-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="2d5de-103">Viestin lähettänyt IP-osoite on [Spamhausin](https://go.microsoft.com/fwlink/p/?linkid=123245)omistamassa estoluettelossa.</span><span class="sxs-lookup"><span data-stu-id="2d5de-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="2d5de-104">Spamhausin estämisen syitä ovat mm. vaarantunut tili, vaarantunut kone, joka jakaa julkisen IP-osoitteen, sekä Internet-palveluntarjoajan käytännöt.</span><span class="sxs-lookup"><span data-stu-id="2d5de-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="2d5de-105">Mahdollisia korjauksia ovat seuraavat:</span><span class="sxs-lookup"><span data-stu-id="2d5de-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="2d5de-106">Jos saapuvat viestit ovat estettyjä, kun hallitset lähdesähköpostipalvelinta, sinun on määritettävä syy ja poistettava esto Spamhaus-sivustosta.</span><span class="sxs-lookup"><span data-stu-id="2d5de-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="2d5de-107">Jos saapuvat viestit on estetty ja IP-lähdeosoite kuuluu jollekulle muulle, osoitteen omistajan on poistettava esto Spamhaus-sivustosta.</span><span class="sxs-lookup"><span data-stu-id="2d5de-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="2d5de-108">Jos IP-osoite on PBL-käytännön estoluettelossa, omistaja voi määrittää toisen staattisen IP-osoitteen tai poistaa osoitteen PBL:sta.</span><span class="sxs-lookup"><span data-stu-id="2d5de-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="2d5de-109">Jos kyse on Microsoftiin yhdistetystä toimialueestasi estetyt lähtevät viestit, voit saada tämän virheen, jos viestit reititetaan kolmannen osapuolen palvelun kautta.</span><span class="sxs-lookup"><span data-stu-id="2d5de-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="2d5de-110">Voit etsiä estettyjen IP-osoitteiden omistajan WHOIS-hakutyökalun avulla.</span><span class="sxs-lookup"><span data-stu-id="2d5de-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
