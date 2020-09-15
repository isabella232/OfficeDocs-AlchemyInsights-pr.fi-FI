---
title: Ulkopuolisten ryhmien poistaminen käytöstä
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704125"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="67ff8-102">Ulkopuolisten ryhmien poistaminen käytöstä</span><span class="sxs-lookup"><span data-stu-id="67ff8-102">How to disable External Groups</span></span>

<span data-ttu-id="67ff8-103">Yammerin ulkoiset viestit käyttää Exchange-siirto sääntöjä (Etbs), jotka estävät yritys tietojen jakamisen.</span><span class="sxs-lookup"><span data-stu-id="67ff8-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="67ff8-104">Jos haluat estää käyttäjiä luomasta ulkoisia ryhmiä, sinun on määritettävä Exchange-siirto sääntö (ETR) ja määritettävä sitten Yammer käyttämään Exchangen siirto sääntöä ulkoisen viestinnän estämiseen.</span><span class="sxs-lookup"><span data-stu-id="67ff8-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="67ff8-105">Kun olet luonut säännön Exchange Online-hallinta keskuksessa, voit määrittää ETR:N käyttämään Yammerissa seuraavia vaiheita:</span><span class="sxs-lookup"><span data-stu-id="67ff8-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="67ff8-106">Kirjaudu Yammeriin todennettuna järjestelmänvalvojana ja siirry **Yammer-hallinta keskuksessa**C- **sisältö-ja tieto turva- \> asetuksiin.**</span><span class="sxs-lookup"><span data-stu-id="67ff8-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="67ff8-107">Valitse **ulkoiset viestit**-kohdassa **Pakota Exchange Onlinen Exchange-siirto säännöt Yammerissa.**</span><span class="sxs-lookup"><span data-stu-id="67ff8-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="67ff8-108">Valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="67ff8-108">Choose **Save**.</span></span>

<span data-ttu-id="67ff8-109">Lisä tietoja on Ohje aiheessa [ulkoiset viestit-toiminnon poistaminen käytöstä Yammer-verkostossa](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="67ff8-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  