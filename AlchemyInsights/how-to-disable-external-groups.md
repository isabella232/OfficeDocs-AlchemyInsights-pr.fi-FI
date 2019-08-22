---
title: Ulkoinen ryhmien poistaminen käytöstä
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
ms.openlocfilehash: 4683a71438ec31f9e9211404a9c66c4e45e0e1df
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36540898"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="babec-102">Ulkoinen ryhmien poistaminen käytöstä</span><span class="sxs-lookup"><span data-stu-id="babec-102">How to disable External Groups</span></span>

<span data-ttu-id="babec-103">Yammer, ulkoinen viestintä koskee Exchange kuljetusta koskevia sääntöjä (ETRs) estää yrityksen tietojen jakamisen ennakoiva ohjausobjektien joukko.</span><span class="sxs-lookup"><span data-stu-id="babec-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="babec-104">Estää käyttäjiä luomasta ulkoisen ryhmät, haluat määrittää Exchange liikenteen sääntö (ETR) ja määritä sitten Yammer Exchange Transport-säännön avulla voit estää ulkoisen viestinnän.</span><span class="sxs-lookup"><span data-stu-id="babec-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="babec-105">Kun olet luonut säännön Exchange Online-hallintakeskukseen, asettaa ETR Yammer sovelletaan seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="babec-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="babec-106">C voit kirjautua Yammer tarkistetut admin, ja **admin center Yammer**- **sisältö- ja \> suojausasetukset.**</span><span class="sxs-lookup"><span data-stu-id="babec-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="babec-107">Valitse **Ulkoisen viestinnän**, **pakottaa Yammer-Exchange Online Exchange liikenteen sääntöjä (ETRs).**</span><span class="sxs-lookup"><span data-stu-id="babec-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="babec-108">Valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="babec-108">Choose **Save**.</span></span>

<span data-ttu-id="babec-109">Lisätietoja on kohdassa [Control ulkoisen viestinnän Yammer verkossa, jossa säännöt Exchange-siirto](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="babec-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  