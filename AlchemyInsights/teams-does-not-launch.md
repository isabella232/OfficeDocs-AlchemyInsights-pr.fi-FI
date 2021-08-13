---
title: Teams ei käynnisty
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813346"
---
# <a name="teams-doesnt-launch"></a>Teams ei käynnisty

Jos yrität avata Microsoft Teams mutta se ei käynnisty koskaan, kokeile seuraavaa:

1. Siirry kansioon **%appdata%\Microsoft\Teams**.
1. Poista kansion sisältö.
1. Käynnistä tietokone uudelleen ja yritä käynnistää Teams.

Sinun on ehkä asennettava Teams. Uudelleenasentaminen:

1. Poista Teams Ohjauspaneelin avulla.
1. Siirry kansioon **%appdata%\Microsoft\Teams\Application Cache.**
1. Poista kansion sisältö.
1. Siirry kansioon **%appdata%\Microsoft\teams\Cache**.
1. Poista kansion sisältö.
1. Käynnistä tietokone uudelleen ja lataa ja asenna Teams.

Jos haluat suorittaa vianmäärityksen vuokraajassasi tietylle käyttäjälle, joka ei voi kirjautua sisään, aloita uusi haku avainsanalla **TeamsUserUnableToSignIn** ja noudata ohjeita.