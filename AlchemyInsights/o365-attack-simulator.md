---
title: 2681 Hyökkäyssimulaattori Microsoft 365:ssä
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506735"
---
# <a name="attack-simulator-in-microsoft-365"></a>Hyökkäyssimulaattori Microsoft 365:ssä

- Puuttuuko Attack Simulator? Attack Simulator edellyttää **Office 365 Advanced Threat Protection Plan 2:ta (ATP-palvelupaketti 2)** tai **Office 365 Enterprise E5:tä.** Attack Simulator **ei** sisälly Office 365 Advanced Threat Protection Plan 1:een (ATP-palvelupaketti 1), Office 365 Enterprise E3:een tai mihinkään Microsoft 365 -sovellukseen yrityksille -tilauksiin.

- Simuloitujen hyökkäysten käynnistämiseen käytettävä tili edellyttää yleisen järjestelmänvalvojan tai suojauksen järjestelmänvalvojan oikeuksia ja mfa-todennusta. Lisätietoja Attack Simulator -vaatimuksista on [tässä ohjeaiheessa](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Tärkeitä asioita tietää **Brute Force Password** hyökkäys simulaatiot:

  - Jos kohdetilillä on mfa käytössä ja salasana on arvattu oikein, tiliä ei näy vaarantuneena (toinen todennuskerroin on epätäydellinen).

  - Salasanatiedoston koko ei voi olla suurempi kuin 10 Mt. Käytä yhtä salasanaa riviä kohden ja lisää tyhjä rivi (rivinvaihto) luettelon viimeisen salasanan jälkeen.

- Tärkeitä asioita, jotka on tiedettävä **Spear Phishing** -liittääksesi simulaatioita:

  - Et voi antaa mukautettua arvoa **tietojenkalastelun kirjautumispalvelimen URL-osoitteelle.**

  - Jos vastaanottaja ilmoittaa viestin tietojenkalasteluksi [Ota raporttiviesti käyttöön -apuohjelman](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) avulla, et ehkä saa ilmoituksia viestistä (koska kyseessä on simuloitu hyökkäys).

- Raportit: Kun simuloitu hyökkäys on valmis, voit tarkastella raporttia valitsemalla **Hyökkäyksen tiedot.**

- Lisätietoja Attack Simulatorin yksityiskohtaisista ohjeista ja uusista ominaisuuksista on [ohjeaiheessa Attack Simulator Microsoft 365 :ssä](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
