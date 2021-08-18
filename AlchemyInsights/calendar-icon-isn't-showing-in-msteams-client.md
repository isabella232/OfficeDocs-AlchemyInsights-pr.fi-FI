---
title: Kalenteri-kuvake ei näy Microsoft Teams asiakasohjelmassa
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
ms.openlocfilehash: edd6b4a2d94b03cf4ae7bf3a8d6332ed94a7e8263aba9df1f9588eecbd0ce05a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54120001"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Kalenteri-kuvake ei näy Microsoft Teams asiakasohjelmassa

**Kalenteri-välilehti** Teams edellyttää Exchange postilaatikon Exchange verkkopalveluiden kautta. Postilaatikon Exchange voi olla Online tai Paikallinen. Jos online-käyttäjä ei  näe Kalenteri-välilehteä, varmista, että heillä on käyttöoikeus Exchange Online ja [että postilaatikko on otettu käyttöön.](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes) Jos käyttäjät ovat kotikäyttäjiä paikallisesti, sinun on vahvistettava, että yhdistelmäkokoonpano on kunnossa. Käytä [yhdistelmämäärityksen ohjattua toimintoa](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) vianmääritystä varten. Huomaa, että [Teams edellyttää Exchange 2016 CU3 -versiota tai uudempaa versiota](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Lisätietoja ja vianmääritysohjeita on kohdassa Microsoft Teams [ja Exchange Server vianmääritys.](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)
