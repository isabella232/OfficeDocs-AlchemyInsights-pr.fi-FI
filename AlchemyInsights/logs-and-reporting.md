---
title: Lokit ja raportointi
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035914"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="8ae83-102">Lokit ja raportointi</span><span class="sxs-lookup"><span data-stu-id="8ae83-102">Logs and Reporting</span></span>

<span data-ttu-id="8ae83-103">[Azure Active Directory -raportoinnin usein kysytyissä](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) kysymyksissä vastataan usein kysyttyihin kysymyksiin Azure Active Directory (Azure AD) -raportoinnista.</span><span class="sxs-lookup"><span data-stu-id="8ae83-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="8ae83-104">Lisätietoja on Azure [Active Directory -raportoinnissa.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)</span><span class="sxs-lookup"><span data-stu-id="8ae83-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="8ae83-105">**Valvontaongelmien vianmääritys**</span><span class="sxs-lookup"><span data-stu-id="8ae83-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="8ae83-106">Jos sinulla on ongelmia joidenkin valvontaaktiviteettien kanssa ja jos puuttuvia toimintoja on [luettelossa,](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)lähetä tukipalvelupyynnön.</span><span class="sxs-lookup"><span data-stu-id="8ae83-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="8ae83-107">Jos sinulla on ongelmia vuokraajan valvontalokien kanssa, lähetä tukipalvelupyynnön.</span><span class="sxs-lookup"><span data-stu-id="8ae83-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="8ae83-108">Jos valvontatoiminnot eivät näy heti Azure-portaalissa, [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) tarkista viivetiedot ja tee tukipyynnön, jos viive ylittää dokumentoidyn viiveen.</span><span class="sxs-lookup"><span data-stu-id="8ae83-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="8ae83-109">Azure AD :n toimintalokien säilytys</span><span class="sxs-lookup"><span data-stu-id="8ae83-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="8ae83-110">Jos et näe kaikkia valitsemiasi päivämäärävälin valvontoja, voit ladata enintään 250 000 riviä (uusimman) kirjautumisen mukaan Azure-portaalista.</span><span class="sxs-lookup"><span data-stu-id="8ae83-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="8ae83-111">Lisätietoja on kohdassa [Valvonta-toimintojen lataaminen.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)</span><span class="sxs-lookup"><span data-stu-id="8ae83-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="8ae83-112">**Kirjautumisongelmien vianmääritys**</span><span class="sxs-lookup"><span data-stu-id="8ae83-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="8ae83-113">Näet viimeisen 30 päivän tiedot vain, jos sinulla on Azure AD Premium (P1 tai P2) -käyttöoikeus vuokraajassasi.</span><span class="sxs-lookup"><span data-stu-id="8ae83-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="8ae83-114">Kirjautumiset ovat käytettävissä vain Azure AD Premium -vuokralaisille.</span><span class="sxs-lookup"><span data-stu-id="8ae83-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="8ae83-115">Se ei ole käytettävissä ilmaisille tai peruskäyttöomistajille.</span><span class="sxs-lookup"><span data-stu-id="8ae83-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="8ae83-116">Jos vuokraajallasi on Premium P1 -käyttöoikeus etkä näe kirjautumisia, [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) tutustu viivetietoomme ja anna tukipyynnön, jos viive ylittää dokumentoidyn viiveen.</span><span class="sxs-lookup"><span data-stu-id="8ae83-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="8ae83-117">Jos et näe kaikkia valitsemasi päivämääräalueen kirjautumisia, huomaa, että voit ladata enintään 250 000 riviä (uusimman) kirjautumisen mukaan Azure-portaalista.</span><span class="sxs-lookup"><span data-stu-id="8ae83-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="8ae83-118">Lisätietoja on [ladattavassa kirjautumisaktiviteetissa.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)</span><span class="sxs-lookup"><span data-stu-id="8ae83-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="8ae83-119">**Suojausraporttien vianmääritys (riskialttiille käyttäjille, riskialttiille kirjautumisille)**</span><span class="sxs-lookup"><span data-stu-id="8ae83-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="8ae83-120">Riskiturvaraporttiin merkityt käyttäjät</span><span class="sxs-lookup"><span data-stu-id="8ae83-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="8ae83-121">Riskialtista kirjautumisraporttia Azure Active Directory -portaalissa</span><span class="sxs-lookup"><span data-stu-id="8ae83-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="8ae83-122">Azure Active Directoryn riskitapahtumat</span><span class="sxs-lookup"><span data-stu-id="8ae83-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
