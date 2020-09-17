---
title: Virhe lähetettäessä sähkö postia, jonka SpamHaus on torjunut
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783800"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="ef779-102">Virhe lähetettäessä sähkö postia: asiakas isäntä on torjunut Spamhausin avulla</span><span class="sxs-lookup"><span data-stu-id="ef779-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="ef779-103">Viestin lähettänyt IP-osoite on [Spamhausin](https://go.microsoft.com/fwlink/p/?linkid=123245)omistama estettyjen luettelossa.</span><span class="sxs-lookup"><span data-stu-id="ef779-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="ef779-104">Syitä, joiden vuoksi spamhaus on saattanut estää, ovat vaarantuneet asiakkuudet, luvatut koneet, jotka jakavat julkisen IP-osoitteen ja Internet-palveluntarjoajan käytännöt.</span><span class="sxs-lookup"><span data-stu-id="ef779-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="ef779-105">Mahdollisia korjauksia ovat seuraavat:</span><span class="sxs-lookup"><span data-stu-id="ef779-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="ef779-106">Jos haluat estää saapuvat viestit, joissa voit hallita lähde Sähkö posti palvelinta, sinun on määritettävä syy ja poistettava lohko Spamhausin verkkosivustosta.</span><span class="sxs-lookup"><span data-stu-id="ef779-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="ef779-107">Estettyjen saapuvien viestien osalta, joihin lähde-IP-osoite kuuluu jollekulle muulle, osoitteen omistajan on poistettava lohko Spamhausin verkkosivustosta.</span><span class="sxs-lookup"><span data-stu-id="ef779-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="ef779-108">Jos IP-osoite on käytäntöjen esto luettelossa (PBL), omistaja voi määrittää eri staattisen IP-osoitteen tai poistaa osoitteen PBL-tiedostosta.</span><span class="sxs-lookup"><span data-stu-id="ef779-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="ef779-109">Voit saada tämän virhe sanoman, kun sähkö posti viesti on kytketty Microsoft-toimi alueelta, jos viestit reititetään kolmannen osapuolen palvelun kautta.</span><span class="sxs-lookup"><span data-stu-id="ef779-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="ef779-110">Voit etsiä torjutun IP-osoitteen omistajan WHOIS-haku työkalun avulla.</span><span class="sxs-lookup"><span data-stu-id="ef779-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
