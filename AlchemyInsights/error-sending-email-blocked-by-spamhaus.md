---
title: Virhe esti SpamHaus sähköpostin lähettäminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 7d6ad2667613ae948a4abcefafe8d91cf89d2418
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402256"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="050c1-102">Virhe lähetettäessä sähköpostia: asiakkaan isäntä esti Spamhaus avulla</span><span class="sxs-lookup"><span data-stu-id="050c1-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="050c1-103">IP-osoite, joka lähetetty viesti on torjuttujen luettelon omistaa [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="050c1-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="050c1-104">Syistä Spamhaus estää tartunnan saaneen tilit ovat tartunnan koneet julkisen IP-osoitteen ja Internet-palveluntarjoajan (ISP) käytäntöjen jakaminen.</span><span class="sxs-lookup"><span data-stu-id="050c1-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="050c1-105">Mahdolliset korjaukset ovat seuraavat:</span><span class="sxs-lookup"><span data-stu-id="050c1-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="050c1-106">Estetty saapuvien viestien, jossa voit määrittää Lähdepalvelimen sähköposti Office 365: ssä sinun on syy ja poistaa lohkon Spamhaus WWW-sivustosta.</span><span class="sxs-lookup"><span data-stu-id="050c1-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="050c1-107">Estetty saapuvien viestien, jossa lähde-IP-osoite kuuluu jollekin toiselle Office 365-osoitteen omistaja on poistettava esto Spamhaus WWW-sivustosta.</span><span class="sxs-lookup"><span data-stu-id="050c1-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="050c1-108">Jos IP-osoite-käytännön Block luetteloon (jaossa PBL), omistaja voi eri staattisen IP-osoitteen tai poistaa osoitteen jaossa PBL.</span><span class="sxs-lookup"><span data-stu-id="050c1-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="050c1-109">Office 365-toimialueen estettyjen lähtevien viestien kohdata tämän virheen, jos Sanomat reititetään 3 osapuolen palvelun kautta.</span><span class="sxs-lookup"><span data-stu-id="050c1-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="050c1-110">WHOIS haku-työkalun avulla voit löytää estetty IP-osoite omistaja.</span><span class="sxs-lookup"><span data-stu-id="050c1-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

