---
title: Kalenteri-kuvake ei näy Microsoft teams-asiakas ohjelmassa
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583530"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a><span data-ttu-id="40dd6-102">Kalenteri-kuvake ei näy Microsoft teams-asiakas ohjelmassa</span><span class="sxs-lookup"><span data-stu-id="40dd6-102">Calendar icon isn't showing in Microsoft Teams client</span></span>

<span data-ttu-id="40dd6-103">Teamsin **kalenteri** -väli lehti edellyttää Exchange-posti laatikon käyttöä Exchange-verkko palveluiden kautta.</span><span class="sxs-lookup"><span data-stu-id="40dd6-103">The **Calendar** Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="40dd6-104">Exchange-posti laatikko voi olla online-tilassa tai paikallisesti.</span><span class="sxs-lookup"><span data-stu-id="40dd6-104">The Exchange mailbox can be Online, or On-Premises.</span></span> <span data-ttu-id="40dd6-105">Jos sinulla on online-käyttäjät, jotka eivät näe **kalenteri** -väli lehteä, varmista, että heillä [on Exchange Online-posti laatikon käyttö oikeus ja että posti laatikko on otettu käyttöön](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="40dd6-105">For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span> <span data-ttu-id="40dd6-106">Jos käyttäjät ovat paikallisessa paikassa, sinun on varmistettava, että yhdistelmä määritykset ovat kunnossa.</span><span class="sxs-lookup"><span data-stu-id="40dd6-106">If your users are homed On-Premises, you need to confirm that your Hybrid configuration is healthy.</span></span> <span data-ttu-id="40dd6-107">Käytä [yhdistelmämäärityksen ohjattua toimintoa](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) vianmääritystä varten.</span><span class="sxs-lookup"><span data-stu-id="40dd6-107">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span> <span data-ttu-id="40dd6-108">Huomaa, että [Teams edellyttää Exchange 2016 CU3 -versiota tai uudempaa versiota](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="40dd6-108">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

<span data-ttu-id="40dd6-109">Lisä tietoja ja vian määritys ohjeita on artikkelissa [Microsoft teamsin ja Exchange Serverin vuorovaikutus ongelmien vian määritys](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span><span class="sxs-lookup"><span data-stu-id="40dd6-109">For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span></span>
