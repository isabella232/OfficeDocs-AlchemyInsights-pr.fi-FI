---
title: Kirjautuminen Microsoft Edge sisään
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
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050691"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Kirjautuminen Microsoft Edge sisään

Microsoft Edge käyttää käyttöjärjestelmän oletustiliä käyttäjän automaattinen kirjautuminen käyttäjän laitteen määritysten mukaan. 

Kunkin laitekokoonpanon ja sen riippuvaisen käyttäjän kirjautumisprosessin skenaariot on kuvattu seuraavassa:

- **Laite on yhdistelmäympäristö /AAD-J:** Tämä asetus on käytettävissä Windows 10, Windows ja sitä vastaavissa palvelinversioissa. Käyttäjät kirjautuvat automaattisesti sisään Azure Active Directory (AD) -tileinsä avulla.
- **Laite on liitetty toimialueeseen:** Tämä asetus on käytettävissä Windows 10, Windows ja sitä vastaavissa palvelinversioissa. Käyttäjät, joilla on toimialuetili, eivät oletusarvoisesti kirjaudu sisään automaattisesti. jos haluat ottaa käyttöön heille automaattisen kirjautumisen, käytä **ConfigureOnPremisesAccountAutoSignIn-käytäntöä.** Jos haluat ottaa automaattisen kirjautumisen käyttöön Azure AD -tileillä, harkitse yhdistelmäympäristön liittämistä heidän laitteisiinsa.
- **Käyttöjärjestelmän oletustili** on Microsoft-tili: Tämä asetus on käytettävissä Windows 10 RS3 :ssa (versio 1709, koontiversio 10.0.16299) ja sitä udemmissa versioissa. Skenaariota ei todennäköisesti esiinny yrityksen laitteissa. Jos käyttöjärjestelmän oletustili on Microsoft-tili, Microsoft Edge käyttäjä kirjautuu automaattisesti sisään Microsoft-tilillä.
 
 
