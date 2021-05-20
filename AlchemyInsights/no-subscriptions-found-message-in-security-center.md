---
title: Suojauskeskuksessa ei löytynyt tilausviestiä
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544105"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Suojauskeskuksessa ei löytynyt tilausviestiä

Jos Microsoft Defender Security Center käytön aikana saat "Tilauksia ei löytynyt" -viestin, se tarkoittaa, että Azure Active Directory (AAD), jolla käyttäjä kirjautuu portaaliin, ei ole Microsoft Defender ATP käyttöoikeutta.  

E5 Windows ja Office E5 -käyttöoikeudet ovat erillisiä käyttöoikeuksia.

Avaa tukitapaus, jos käyttöoikeus on ostettu, mutta sitä ei ole määritetty tähän AAD-esiintymään. Sinulla on joko: <br/>
-   Mahdollinen käyttöoikeuksien valmisteluongelma.<br/>
-   Olet vahingossa valmistella käyttöoikeuden eri Microsoft AAD:lle kuin palveluun todentamiseen käytetty käyttöoikeus.