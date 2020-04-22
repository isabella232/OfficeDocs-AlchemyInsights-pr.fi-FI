---
title: Virhe lähetettäessä Roskapostin estämiä sähköpostiviestejä
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714255"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="67761-102">Virhe lähetettäessä sähköpostia: Asiakkaan isäntä estetty Roskapostin avulla</span><span class="sxs-lookup"><span data-stu-id="67761-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="67761-103">Viestin lähettänyt IP-osoite on [Spamhausin](https://go.microsoft.com/fwlink/p/?linkid=123245)omistamassa estoluettelossa.</span><span class="sxs-lookup"><span data-stu-id="67761-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="67761-104">Spamhausin estämisen syitä ovat vaarantuneet tilit, vaarantuneet koneet, joilla on julkinen IP-osoite, sekä Internet-palveluntarjoajan käytännöt.</span><span class="sxs-lookup"><span data-stu-id="67761-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="67761-105">Mahdollisia korjauksia ovat:</span><span class="sxs-lookup"><span data-stu-id="67761-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="67761-106">Estetyt saapuvat viestit, joissa hallitset lähdesähköpostipalvelinta, sinun on määritettävä syy ja poistettava lohko Spamhaus-sivustosta.</span><span class="sxs-lookup"><span data-stu-id="67761-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="67761-107">Estetyt saapuvat viestit, joissa lähteen IP-osoite kuuluu jollekulle muulle, osoitteen omistajan on poistettava lohko Spamhaus-sivustosta.</span><span class="sxs-lookup"><span data-stu-id="67761-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="67761-108">Jos IP-osoite on PBL(Policy Block List) -luettelossa, omistaja voi määrittää toisen staattisen IP-osoitteen tai poistaa osoitteen PBL:stä.</span><span class="sxs-lookup"><span data-stu-id="67761-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="67761-109">Jos toimialueeltasi on estettyjä lähteviä viestejä, jotka on yhdistetty Microsoftiin, tämä virhe ilmenee, jos viestit reititetään kolmannen osapuolen palvelun kautta.</span><span class="sxs-lookup"><span data-stu-id="67761-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="67761-110">Voit etsiä estetyn IP-osoitteen omistajan WHOIS-hakutyökalun avulla.</span><span class="sxs-lookup"><span data-stu-id="67761-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
