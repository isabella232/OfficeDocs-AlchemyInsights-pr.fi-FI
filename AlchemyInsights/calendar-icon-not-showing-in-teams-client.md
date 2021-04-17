---
title: Kalenteri-kuvake ei näy Teams-asiakasohjelmassa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819950"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="747aa-102">Kalenteri-kuvake ei näy Teams-asiakasohjelmassa</span><span class="sxs-lookup"><span data-stu-id="747aa-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="747aa-103">Teamsin Kalenteri-välilehti edellyttää Exchange-postilaatikon käyttöä Exchange-verkkopalvelujen kautta.</span><span class="sxs-lookup"><span data-stu-id="747aa-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="747aa-104">Exchange-postilaatikko voi olla online-tilassa tai paikallinen.</span><span class="sxs-lookup"><span data-stu-id="747aa-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="747aa-105">Jos online-käyttäjät eivät näe Kalenteri-välilehteä, varmista, että heillä [on Exchange Online -postilaatikon käyttöoikeus ja että postilaatikko on otettu käyttöön](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="747aa-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="747aa-106">Jos käyttäjällä on kelvollinen postilaatikko Exchange Onlinessa, mutta hän ei edelleenkään näe Kalenteri-välilehteä, kyse voi olla verkko-ongelmasta.</span><span class="sxs-lookup"><span data-stu-id="747aa-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="747aa-107">Käytä [Microsoft Remote Connectivity Analyzeria](https://testconnectivity.microsoft.com/) ja suorita kyseiselle käyttäjälle **Microsoft Exchange -verkkopalveluyhteystestit**.</span><span class="sxs-lookup"><span data-stu-id="747aa-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="747aa-108">Tarkista lopuksi [Teams-sovellukset – Sovelluksen määrityskäytännöt](https://admin.teams.microsoft.com/policies/app-setup) sen varmistamiseksi, ettei Kalenteri-sovellusta ole poistettu käyttäjään sovellettavasta käytännöstä (luultavimmin **Yleinen (organisaation laajuinen oletus)**.</span><span class="sxs-lookup"><span data-stu-id="747aa-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="747aa-109">Jos käyttäjät ovat paikallisia, varmista, että yhdistelmämäärityksesi on kunnossa.</span><span class="sxs-lookup"><span data-stu-id="747aa-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="747aa-110">Käytä [yhdistelmämäärityksen ohjattua toimintoa](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) vianmääritystä varten.</span><span class="sxs-lookup"><span data-stu-id="747aa-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="747aa-111">Huomaa, että [Teams edellyttää Exchange 2016 CU3 -versiota tai uudempaa versiota](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="747aa-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
