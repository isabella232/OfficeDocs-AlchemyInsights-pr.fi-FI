---
title: Petosten paljastamista koskeva turvallisuus Vihje vianmääritys tarkistaa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 24842e8cc5c6e47fb0eb637e6a3211637ede1ed8
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28287263"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="ae70a-102">Petosten paljastamista koskeva turvallisuus Vihje vianmääritys tarkistaa</span><span class="sxs-lookup"><span data-stu-id="ae70a-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="ae70a-p101">Jos olet käytön turvallisuus kärki, joka sanoo ”lähettäjä meidän petosten havaitseminen tarkastukset epäonnistui ja saattaa olla kuka ne ilmeisesti” ja sitten lähettäjä ei läpäissyt DKIM- tai SPF käyttöoikeuden tarkastukset. Paras tapa ratkaista tämä on lähettäjän valtuuttaa itse. Jos lähettäjä lähettää puolestasi, sinun tarvitse antaa luvan SPF-tietueen lisäämällä lähettäjän IP-osoite.</span><span class="sxs-lookup"><span data-stu-id="ae70a-p101">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks. The best method to resolve this is for the sender to authorize themselves. If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="ae70a-106">Saat lisätietoja [Punainen (epäilyttäviä) turvallisuuden petosten paljastamista koskeva vihje vianmääritys tarkistaa](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="ae70a-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="ae70a-107">Seuraavassa on muita linkkejä, jotka auttavat:</span><span class="sxs-lookup"><span data-stu-id="ae70a-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="ae70a-108">Kuinka Office 365 käyttää lähettäjän policy framework (SPF) tietojen väärentämisen estämiseksi.</span><span class="sxs-lookup"><span data-stu-id="ae70a-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/en-us/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="ae70a-109">SPF-tietueen määrittäminen Office 365:ssä osoitehuijausten estämiseksi</span><span class="sxs-lookup"><span data-stu-id="ae70a-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/en-us/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

