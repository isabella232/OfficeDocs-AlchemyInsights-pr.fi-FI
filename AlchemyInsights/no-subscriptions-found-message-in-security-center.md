---
title: Suojauskeskuksesta ei löytynyt tilauksia
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
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713602"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Suojauskeskuksesta ei löytynyt tilauksia

Jos saat Microsoft Defender Security Centeriä käytön aikana viestin "Tilauksia ei löytynyt", se tarkoittaa, että Azure Active Directory (AAD), jolla käyttäjä kirjautuu portaaliin, ei ole Microsoft Defender ATP -käyttöoikeutta.  

Windows E5- ja Office E5 -käyttöoikeudet ovat erillisiä käyttöoikeuksia.

Avaa tukitapaus, jos käyttöoikeus on ostettu, mutta sitä ei ole määritetty tähän AAD-esiintymään. Sinulla on jompikumpi seuraavista: <br/>
-   Mahdollinen käyttöoikeuden valmisteluongelma.<br/>
-   Olet vahingossa valmistella käyttöoikeuden eri Microsoft AAD:lle kuin palveluun todentamisessa käytetty käyttöoikeus.