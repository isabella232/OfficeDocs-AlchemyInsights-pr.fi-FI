---
title: Kalenteri-kuvake ei näy Teams-asiakasohjelmassa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931980"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Kalenteri-kuvake ei näy Teams-asiakasohjelmassa

Teamsin Kalenteri-välilehti edellyttää Exchange-postilaatikon käyttöä Exchange-verkkopalvelujen kautta. Exchange-postilaatikko voi olla online-tilassa tai paikallinen. Jos online-käyttäjät eivät näe Kalenteri-välilehteä, varmista, että heillä [on Exchange Online -postilaatikon käyttöoikeus ja että postilaatikko on otettu käyttöön](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Jos käyttäjällä on kelvollinen postilaatikko Exchange Onlinessa, mutta hän ei edelleenkään näe Kalenteri-välilehteä, kyse voi olla verkko-ongelmasta. Käytä [Microsoft Remote Connectivity Analyzeria](https://testconnectivity.microsoft.com/) ja suorita kyseiselle käyttäjälle **Microsoft Exchange -verkkopalveluyhteystestit**.

Tarkista lopuksi [Teams-sovellukset – Sovelluksen määrityskäytännöt](https://admin.teams.microsoft.com/policies/app-setup) sen varmistamiseksi, ettei Kalenteri-sovellusta ole poistettu käyttäjään sovellettavasta käytännöstä (luultavimmin **Yleinen (organisaation laajuinen oletus)**.

Jos käyttäjät ovat paikallisia, varmista, että yhdistelmämäärityksesi on kunnossa. Käytä [yhdistelmämäärityksen ohjattua toimintoa](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) vianmääritystä varten.

Huomaa, että [Teams edellyttää Exchange 2016 CU3 -versiota tai uudempaa versiota](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
