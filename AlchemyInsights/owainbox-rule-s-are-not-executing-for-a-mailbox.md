---
title: 1332 OWA - Saapuneet-kansion sääntöjen ei suoriteta postilaatikkoon
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9e782faa59bb9a16c271f7c46c79635961e88aed
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/22/2019
ms.locfileid: "30784339"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="1c939-102">Saapuneet-sääntö ei toimi odotetulla tavalla</span><span class="sxs-lookup"><span data-stu-id="1c939-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="1c939-103">Tarkista seuraavat asetukset:</span><span class="sxs-lookup"><span data-stu-id="1c939-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="1c939-104">Sanoma voidaan uudellenohjata, välitettyjen ja vastattujen automaattisesti Saapuneet-kansion sääntöjen perusteella vain kerran.</span><span class="sxs-lookup"><span data-stu-id="1c939-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="1c939-105">Uudelleenohjataan sääntö (Saapuneet-kansion sääntö tai sähköpostin virtaussäännön, tunnetaan myös nimellä liikenteen sääntö) voit lisätä enintään kymmenen välityksen vastaanottajien viestin.</span><span class="sxs-lookup"><span data-stu-id="1c939-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="1c939-106">Lisätietoja [kirjauskansion, kuljetus- ja Saapuneet-kansion säännön rajat](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="1c939-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="1c939-107">Vaihtoehtoinen lokiin postilaatikon Saapuneet-kansion säännöt eivät toimi.</span><span class="sxs-lookup"><span data-stu-id="1c939-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="1c939-108">Saat lisätietoja vaihtoehtoinen lokiin postilaatikon [Vaihtoehtoinen lokiin postilaatikon](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="1c939-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="1c939-109">Voit korjata nämä ongelmat, katso [kt 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="1c939-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="1c939-110">Jos edellä kuvatut ongelmat eivät käytä, suorita Saapuneet-kansion säännön diagnostisen raportin ennen ongelmasta Microsoft Support Eskaloi:</span><span class="sxs-lookup"><span data-stu-id="1c939-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="1c939-111">Avaa postilaatikon Outlook Web ja **asetukset** \> **asetukset** \> **Järjestä sähköposti** \> **Saapuneet-kansion sääntöjä**.</span><span class="sxs-lookup"><span data-stu-id="1c939-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="1c939-112">Valitse sivun alareunassa **Jos säännöt eivät toimi voit Diagnostiikkaraportin luominen napsauttamalla tätä**.</span><span class="sxs-lookup"><span data-stu-id="1c939-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    
