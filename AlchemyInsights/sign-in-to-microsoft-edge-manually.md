---
title: Microsoft Edgeen kirjautuminen manuaalisesti
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
- "8332"
- "9004625"
ms.openlocfilehash: f380d09dc14788205638cdee6aebe0b084ecab2f
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398654"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Microsoft Edgeen kirjautuminen manuaalisesti

Jos käyttäjä ei ole kirjautuneena automaattisesti ensimmäisen käyttökokemuksen aikana, käyttäjä voi kirjautua sisään manuaalisesti selaimen asetusten tai käyttäjätietojen pikaikkunan kautta. Jos haluat hallita kirjautumista, käytä seuraavia käytäntöjä:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) – Voit varmistaa, että käyttäjällä on aina työprofiili Microsoft Edgessä.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) – Voit rajoittaa kirjautumisen luotettujen tilien joukkoon.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) – Jos haluat poistaa kirjautumisen käytöstä tai pakottaa käyttäjät kirjautumaan sisään.

