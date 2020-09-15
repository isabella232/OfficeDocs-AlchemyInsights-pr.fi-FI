---
title: 182 Suorita SaRA, jos haluat diagnosoida ja ratkaista Outlookin todennus ongelmat
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "182"
- "1800012"
ms.assetid: a3a5ea91-6989-4616-9290-c7b24484e8c8
ms.openlocfilehash: aa1e831eac829f3bd35f34e2fbe34923c5af0d3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47802018"
---
# <a name="use-sara-to-diagnose-and-resolve-outlook-authentication-issues"></a><span data-ttu-id="4a088-102">Outlookin todennusongelmien vianmääritys ja ratkaiseminen TPA-toiminnon avulla</span><span class="sxs-lookup"><span data-stu-id="4a088-102">Use SaRA to diagnose and resolve Outlook authentication issues</span></span>

<span data-ttu-id="4a088-103">**Huomautus**: Tarkista, onko organisaatiollesi käytössä [tieto turvan oletus asetukset](https://aka.ms/securitydefaults) .</span><span class="sxs-lookup"><span data-stu-id="4a088-103">**Note**: Please check to see whether [security defaults](https://aka.ms/securitydefaults) is enabled for your organization.</span></span> <span data-ttu-id="4a088-104">Jos vuokraaja on luotu 21. loka kuuta jälkeen, 2019 ja Outlook pyytää sinulta toistuvasti Sala sanaa, sinulla voi olla käytössä vuokraajapalvelussasi olevat **turvallisuusasetukset** .</span><span class="sxs-lookup"><span data-stu-id="4a088-104">If your tenant was created after October 21st, 2019 and your Outlook is repeatedly asking you for a password, you may have **security defaults** enabled in your tenant.</span></span>

<span data-ttu-id="4a088-105">Suosittelemme, että käytät [Outlook pyytää edelleen Sala sanan](https://aka.ms/SaRA-OutlookPwdPrompt-Alchemy) diagnostiikkaa haavoittuvuuden sisältävän koneen kanssa, jotta voit tehdä vian määrityksen, jossa Outlook pyytää Sala sanaa jatkuvasti.</span><span class="sxs-lookup"><span data-stu-id="4a088-105">We highly recommend you use the [Outlook keeps asking for my password](https://aka.ms/SaRA-OutlookPwdPrompt-Alchemy) diagnostic on the affected machine to troubleshoot issues where Outlook continually prompts for a password.</span></span> <span data-ttu-id="4a088-106">Tämä [SaRA](https://diagnostics.office.com/#/) -diagnostiikka toiminto suorittaa automaattiset tarkistukset ja palauttaa mahdollisia ratkaisuja, joiden avulla voit korjata havaitut ongelmat.</span><span class="sxs-lookup"><span data-stu-id="4a088-106">This [SaRA](https://diagnostics.office.com/#/) diagnostic does automated checks and returns possible solutions for you to use to address any detected issues.</span></span>
