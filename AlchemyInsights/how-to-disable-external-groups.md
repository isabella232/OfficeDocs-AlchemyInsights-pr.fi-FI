---
title: Ulkoisten ryhmien poistaminen käytöstä
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720765"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="bf47f-102">Ulkoisten ryhmien poistaminen käytöstä</span><span class="sxs-lookup"><span data-stu-id="bf47f-102">How to disable External Groups</span></span>

<span data-ttu-id="bf47f-103">Yammerin ulkoiset viestit käyttävät Exchange Transport Rules (ETRs) -sääntöjä, jotka ovat joukko ennakoivia ohjausobjekteja, jotka estävät yrityksen tietojen jakamisen.</span><span class="sxs-lookup"><span data-stu-id="bf47f-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="bf47f-104">Jotta voit estää käyttäjiä luomasta ulkoisia ryhmiä, sinun on määritettävä Exchange-siirtosääntö (ETR) ja määritettävä Yammer estämään ulkoiset viestit Exchange Transport -säännön avulla.</span><span class="sxs-lookup"><span data-stu-id="bf47f-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="bf47f-105">Kun olet luonut säännön Exchange Online -hallintakeskuksessa, määritä ETR-arvo Yammerissa seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="bf47f-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="bf47f-106">Kirjaudu Yammeriin vahvistetuna järjestelmänvalvojana ja siirry **Yammer-hallintakeskukseen**kohtaan C \*\*Content and Security Settings (C-sisältö- ja suojausasetukset). \> \*\*</span><span class="sxs-lookup"><span data-stu-id="bf47f-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="bf47f-107">Valitse **Ulkoiset viestit -kohdassa** **Pakota Exchange Online Exchange -siirtosäännöt (Etr) Yammerissa.**</span><span class="sxs-lookup"><span data-stu-id="bf47f-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="bf47f-108">Valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="bf47f-108">Choose **Save**.</span></span>

<span data-ttu-id="bf47f-109">Lisätietoja on [ohjeaiheessa Ulkoisten viestien poistaminen käytöstä Yammer-verkossa](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="bf47f-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  