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
# <a name="logs-and-reporting"></a>Lokit ja raportointi

[Azure Active Directory -raportoinnin usein kysytyissä](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) kysymyksissä vastataan usein kysyttyihin kysymyksiin Azure Active Directory (Azure AD) -raportoinnista. Lisätietoja on Azure [Active Directory -raportoinnissa.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)

**Valvontaongelmien vianmääritys**

1. Jos sinulla on ongelmia joidenkin valvontaaktiviteettien kanssa ja jos puuttuvia toimintoja on [luettelossa,](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)lähetä tukipalvelupyynnön.
2. Jos sinulla on ongelmia vuokraajan valvontalokien kanssa, lähetä tukipalvelupyynnön.
3. Jos valvontatoiminnot eivät näy heti Azure-portaalissa, [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) tarkista viivetiedot ja tee tukipyynnön, jos viive ylittää dokumentoidyn viiveen.
4. [Azure AD :n toimintalokien säilytys](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. Jos et näe kaikkia valitsemiasi päivämäärävälin valvontoja, voit ladata enintään 250 000 riviä (uusimman) kirjautumisen mukaan Azure-portaalista. Lisätietoja on kohdassa [Valvonta-toimintojen lataaminen.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)

**Kirjautumisongelmien vianmääritys**

1. Näet viimeisen 30 päivän tiedot vain, jos sinulla on Azure AD Premium (P1 tai P2) -käyttöoikeus vuokraajassasi.
2. Kirjautumiset ovat käytettävissä vain Azure AD Premium -vuokralaisille. Se ei ole käytettävissä ilmaisille tai peruskäyttöomistajille.
3. Jos vuokraajallasi on Premium P1 -käyttöoikeus etkä näe kirjautumisia, [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) tutustu viivetietoomme ja anna tukipyynnön, jos viive ylittää dokumentoidyn viiveen.
4. Jos et näe kaikkia valitsemasi päivämääräalueen kirjautumisia, huomaa, että voit ladata enintään 250 000 riviä (uusimman) kirjautumisen mukaan Azure-portaalista. Lisätietoja on [ladattavassa kirjautumisaktiviteetissa.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)

**Suojausraporttien vianmääritys (riskialttiille käyttäjille, riskialttiille kirjautumisille)**

1. [Riskiturvaraporttiin merkityt käyttäjät](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [Riskialtista kirjautumisraporttia Azure Active Directory -portaalissa](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [Azure Active Directoryn riskitapahtumat](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
