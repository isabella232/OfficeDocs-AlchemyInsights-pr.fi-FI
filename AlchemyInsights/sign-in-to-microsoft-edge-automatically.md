---
title: Kirjautuminen Microsoft Edgeen automaattisesti
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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677236"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Kirjautuminen Microsoft Edgeen automaattisesti

Microsoft Edge käyttää käyttö järjestelmän oletus tiliä kirjautuessaan automaattisesti käyttäjän laitteeseen sen mukaan, miten käyttäjän laite on määritetty. 

Seuraavassa kuvataan kunkin laite tyypin ja sen riippuvaisen käyttäjän kirjautumisprosessin skenaariot:

1. **Laite on yhdistelmä/AAD-J**: Tämä vaihto ehto on käytettävissä Windows 10-, alatason Windows-ja sitä vastaavissa palvelin versioissa. Käyttäjät kirjataan automaattisesti sisään Azure Active Directory (AD)-tileihinsä.
2. **Laite on liitetty toimi alueeseen**: Tämä asetus on käytettävissä Windows 10-, alatason Windows-ja sitä vastaavissa palvelin versioissa. Oletusarvoisesti käyttäjät, joilla on toimi alue tiliä, eivät ole kirjautuneet sisään automaattisesti. Jos haluat ottaa automaattisen kirjautumisen käyttöön, käytä **Configureonenpremisesaccountautosigni** -käytäntöä. Jos haluat ottaa käyttöön automaattisen kirjautumisen käyttäjille, joilla on Azure AD-tilisi, harkitse hybridi-liittymistään laitteisiinsa.
3. **Käyttö järjestelmän oletus tili on Microsoft-tili**: Tämä vaihto ehto on käytettävissä Windows 10 RS3 (version 1709, koonti versio 10.0.16299) ja uudemmissa versioissa. Skenaario ei todennäköisesti toteudu yritys laitteissa. Jos käyttö järjestelmän oletus tili on Microsoft-tili, Microsoft Edge automaattisesti kirjautuu sisään Microsoft-tilillä.
 
 
