---
title: Microsoft Edgeen kirjautuminen automaattisesti
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398726"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Microsoft Edgeen kirjautuminen automaattisesti

Microsoft Edge käyttää käyttöjärjestelmän oletustiliä käyttäjän automaattinen kirjautuminen käyttäjän laitteen määritysten mukaan. 

Kunkin laitekokoonpanon ja sen riippuvaisen käyttäjän kirjautumisprosessin skenaariot on kuvattu alla:

- **Laite on yhdistelmäympäristö/AAD-J:** Tämä asetus on käytettävissä Windows 10:ssä, windowsissa ja sitä vastaavissa palvelinversioissa. Käyttäjät kirjautuvat automaattisesti Azure Active Directory (AD) -tileinsä avulla.
- **Laite on liitetty toimialueeseen:** Tämä asetus on käytettävissä Windows 10:ssä, Windowsissa ja sitä vastaavissa palvelinversioissa. Käyttäjät, joilla on toimialuetili, eivät oletusarvoisesti kirjaudu sisään automaattisesti. jos haluat ottaa automaattisen kirjautumisen käyttöön, käytä **ConfigureOnPremisesAccountAutoSignIn-käytäntöä.** Jos haluat ottaa automaattisen kirjautumisen käyttöön Azure AD -tilejä käyttäjillä, harkitse yhdistelmäympäristön liittämistä heidän laitteisiinsa.
- **Käyttöjärjestelmän oletustili** on Microsoft-tili: Tämä asetus on käytettävissä Windows 10 RS3:ssa (versio 1709, koontiversio 10.0.16299) ja myommissa versioissa. Skenaariota ei todennäköisesti ilmene yrityslaitteilla. Jos käyttöjärjestelmän oletustili on Microsoft-tili, Microsoft Edge kirjautuu automaattisesti sisään käyttäjälle Microsoft-tilillä.
 
 
