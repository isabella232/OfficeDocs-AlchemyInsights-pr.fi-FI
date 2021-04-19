---
title: DLP:n käyttäminen siirtosäännöissä
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
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827213"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="0c96d-102">DLP:n käyttäminen siirtosäännöissä</span><span class="sxs-lookup"><span data-stu-id="0c96d-102">Using DLP in transport rules</span></span>

<span data-ttu-id="0c96d-103">Jos haluat integroida tietojen menetyksen estämisen (DLP) olemassa olevaan siirtoon, käytä siirtosäännön asetuksissa ehtoa "**Jos viesti sisältää... luottamuksellisia tietoja**".</span><span class="sxs-lookup"><span data-stu-id="0c96d-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="0c96d-104">**Saat lisätietoja seuraavasta artikkelista:**</span><span class="sxs-lookup"><span data-stu-id="0c96d-104">**For more details, see:**</span></span>

- <span data-ttu-id="0c96d-105">Integroidut luottamukselliset DLP-tietotyypit siirtosäännöissä: [Luottamuksellisten tietojen sääntöjen integroiminen](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="0c96d-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="0c96d-106">Voit myös testata sääntöä käytännön testauksen kanssa tai ilman sitä käyttämällä sääntöön testitilaa.</span><span class="sxs-lookup"><span data-stu-id="0c96d-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="0c96d-107">Odota 30 minuuttia säännön luomisen jälkeen ennen sen testausta.</span><span class="sxs-lookup"><span data-stu-id="0c96d-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="0c96d-108">Tutustu artikkeliin [Postinkulun ja siirtosääntöjen testaaminen](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="0c96d-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="0c96d-109">**Huomautus**: Jos yrität ottaa uutta siirtosääntöjä sisältävää DLP-käytäntöä käyttöön EAC:ssä, saat ohjeita artikkelista [DLP-käytännöt tietoturva- ja yhteensopivuuskeskuksessa](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="0c96d-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
