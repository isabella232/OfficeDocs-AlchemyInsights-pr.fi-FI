---
title: Ulkoisten ryhmien poistaminen käytöstä
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/25/2019
ms.locfileid: "36739490"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="2fc26-102">Ulkoisten ryhmien poistaminen käytöstä</span><span class="sxs-lookup"><span data-stu-id="2fc26-102">How to disable External Groups</span></span>

<span data-ttu-id="2fc26-103">Yammerin ulkoinen viestintä käyttää Exchange-liikenne sääntöjä (ETF), joka on joukko ennakoivia ohjaus objekteja, jotka estävät yritys tietojen yhteistoiminnan.</span><span class="sxs-lookup"><span data-stu-id="2fc26-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="2fc26-104">Jotta käyttäjät eivät voi luoda ulkoisia ryhmiä, sinun on määritettävä Exchange-siirto sääntö (ETR) ja määritettävä sitten Yammer käyttämään Exchange-siirto sääntöä ulkoisen Sanoman välityksen estämiseksi.</span><span class="sxs-lookup"><span data-stu-id="2fc26-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="2fc26-105">Kun olet luonut säännön Exchange Online-hallinta keskuksessa, määritä ETR-sovellus Yammerissa seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="2fc26-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="2fc26-106">Kirjaudu Yammeriin todennas-järjestelmänvalvojana ja **Yammerin hallinta keskuksessa**kohtaan C **Content ja Security \> Security Settings.**</span><span class="sxs-lookup"><span data-stu-id="2fc26-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="2fc26-107">Valitse **ulkoiset viestit**-kohdassa **Pakota Exchange Online Exchange-siirto sääntösi (ETR) Yammerissa.**</span><span class="sxs-lookup"><span data-stu-id="2fc26-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="2fc26-108">Valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="2fc26-108">Choose **Save**.</span></span>

<span data-ttu-id="2fc26-109">Lisä tietoja on kohdassa [ulkoisten viestien poistaminen käytöstä Yammer-verkossa](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="2fc26-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  