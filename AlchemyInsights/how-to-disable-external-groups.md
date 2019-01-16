---
title: Ulkoinen ryhmien poistaminen käytöstä
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4807dbfbabcea1f13785bd39bb48e4bbaa8d0f0f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28286551"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="608d5-102">Ulkoinen ryhmien poistaminen käytöstä</span><span class="sxs-lookup"><span data-stu-id="608d5-102">How to disable External Groups</span></span>

<span data-ttu-id="608d5-p101">Yammer, ulkoinen viestintä koskee Exchange kuljetusta koskevia sääntöjä (ETRs) estää yrityksen tietojen jakamisen ennakoiva ohjausobjektien joukko. Estää käyttäjiä luomasta ulkoisen ryhmät, haluat määrittää Exchange liikenteen sääntö (ETR) ja määritä sitten Yammer Exchange Transport-säännön avulla voit estää ulkoisen viestinnän.</span><span class="sxs-lookup"><span data-stu-id="608d5-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="608d5-105">Kun olet luonut säännön Exchange Online-hallintakeskukseen, asettaa ETR Yammer sovelletaan seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="608d5-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="608d5-106">C voit kirjautua Yammer tarkistetut admin, ja **admin center Yammer**- **ontent ja \> suojausasetukset.**</span><span class="sxs-lookup"><span data-stu-id="608d5-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="608d5-107">Valitse **Ulkoisen viestinnän**, **pakottaa Yammer-Exchange Online Exchange liikenteen sääntöjä (ETRs).**</span><span class="sxs-lookup"><span data-stu-id="608d5-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="608d5-108">Valitse **Save** (Tallenna).</span><span class="sxs-lookup"><span data-stu-id="608d5-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="608d5-109">Lisätietoja on kohdassa [Control ulkoisen viestinnän Yammer verkossa, jossa säännöt Exchange-siirto](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="608d5-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

