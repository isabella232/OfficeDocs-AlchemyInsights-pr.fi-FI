---
title: Vian määritys suojaus vihjeestä petosten havaitsemisen tarkistukset
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658407"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="d802d-102">Vian määritys suojaus vihjeestä petosten havaitsemisen tarkistukset</span><span class="sxs-lookup"><span data-stu-id="d802d-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="d802d-103">Jos saat turva vihjeen, jossa lukee "lähettäjä ei onnistunut huijausten havaitsemisessa, eikä se ehkä ole", lähettäjä ei voinut siirtää DKIM-tai SPF-todennus tarkistuksia.</span><span class="sxs-lookup"><span data-stu-id="d802d-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="d802d-104">Paras tapa korjata tämä on se, että lähettäjä valtuuttaa itsensä.</span><span class="sxs-lookup"><span data-stu-id="d802d-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="d802d-105">Jos lähettäjä lähettää viestin puolestasi, sinun on valtuutettava heidät lisäämällä lähettäjän IP-osoite SPF-tietueeseen.</span><span class="sxs-lookup"><span data-stu-id="d802d-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="d802d-106">Lisä tietoja [on kohdassa punaisen (epäilyttävän) suojaus vihjeen vian määritys petosten havaitsemis tarkistuksissa](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="d802d-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="d802d-107">Seuraavassa on joitakin muita linkkejä, joista voi olla apua:</span><span class="sxs-lookup"><span data-stu-id="d802d-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="d802d-108">Tietoja siitä, miten Microsoft käyttää SPF (lähettäjän Policy Framework)-järjestelmää tietojen väärentämisen estämiseen</span><span class="sxs-lookup"><span data-stu-id="d802d-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="d802d-109">SPF-osoitteen määrittäminen estämään tietojen väärentämisen estäminen</span><span class="sxs-lookup"><span data-stu-id="d802d-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
