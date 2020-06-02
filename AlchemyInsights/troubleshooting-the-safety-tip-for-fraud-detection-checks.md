---
title: Petostenhavaitsemistarkistusten turvallisuusvihjeen vianmääritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504980"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="45bf6-102">Petostenhavaitsemistarkistusten turvallisuusvihjeen vianmääritys</span><span class="sxs-lookup"><span data-stu-id="45bf6-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="45bf6-103">Jos saat turvallisuusvihjeen, jossa lukee "Lähettäjä ei läpäissyt petosten havaitsemistarkistuksia eikä ehkä ole sitä, kuka ne näyttävät olevan", lähettäjä ei läpäissyt DKIM- tai SPF-todennustarkistuksia.</span><span class="sxs-lookup"><span data-stu-id="45bf6-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="45bf6-104">Paras tapa ratkaista tämä on, että lähettäjä valtuuttaa itsensä.</span><span class="sxs-lookup"><span data-stu-id="45bf6-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="45bf6-105">Jos lähettäjä lähettää sen puolestasi, sinun on valtuutettava se lisäämällä lähettäjän IP-osoite SPF-tietueeseesi.</span><span class="sxs-lookup"><span data-stu-id="45bf6-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="45bf6-106">Lisätietoja on [ohjeaiheessa Petosten havaitsemisen vianmääritys punaisen (epäilyttävän) turvallisuusvihjeen](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) vianmääritys.</span><span class="sxs-lookup"><span data-stu-id="45bf6-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="45bf6-107">Seuraavassa on joitakin muita linkkejä, jotka voivat auttaa:</span><span class="sxs-lookup"><span data-stu-id="45bf6-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="45bf6-108">Microsoftin tapa estää väärentäminen lähettäjän käytäntökehyksellä (SPF)</span><span class="sxs-lookup"><span data-stu-id="45bf6-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="45bf6-109">SPF:n määrittäminen estämään väärentäminen</span><span class="sxs-lookup"><span data-stu-id="45bf6-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
