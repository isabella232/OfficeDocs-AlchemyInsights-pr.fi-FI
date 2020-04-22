---
title: 2681 Hyökkäys Simulaattori Microsoft 365:ssä
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
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713463"
---
# <a name="attack-simulator-in-microsoft-365"></a>Hyökkäys Simulator Microsoft 365:ssä

- Kaipaatko Attack Simulatoria? Attack Simulator edellyttää **Office 365 Advanced Threat Protection Plan 2:ta (ATP-sopimus 2)** tai **Office 365 Enterprise E5:tä.** Attack Simulator **ei** sisälly Office 365 Advanced Threat Protection Plan 1:een (ATP-palvelupaketti 1), Office 365 Enterprise E3:een tai mihinkään Microsoft 365 Apps for Business -tilaukseen.

- Simuloidun hyökkäyksen käynnistämiseen käytettävä tili edellyttää yleisiä järjestelmänvalvojan tai suojauksen järjestelmänvalvojan oikeuksia ja monivaiheista todennusta.The account you use to launch simuloituja hyökkäyksiä edellyttää yleisiä järjestelmänvalvojan tai suojauksen järjestelmänvalvojan oikeuksia ja monivaiheinen todennus (MFA). Lisätietoja Attack Simulator -vaatimuksista on [tässä ohjeaiheessa](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Tärkeää tietoa **Brute Force Salasana** hyökkäys simulaatioita:

  - Jos kohdetilillä on mfa käytössä ja salasana on arvattu oikein, tiliä ei näytetä vaarantunut (toinen todennuskerroin on epätäydellinen).

  - Salasanatiedosto ei voi olla suurempi kuin 10 Mt. Käytä yhtä salasanaa riviä kohden ja sisällytä tyhjä rivi (rivinvaihto) luettelon viimeisen salasanan jälkeen.

- Tärkeitä asioita tietää **Spear Phishing** liittää simulaatioita:

  - **Tietojenkalastelun kirjautumispalvelimen URL-osoitteelle**ei voi antaa mukautettua arvoa.

  - Jos vastaanottaja käyttää [Ota raporttiviesti käyttöön -apuohjelmaa](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) ilmoittaakseen viestin tietojenkalasteluksi, et ehkä saa ilmoituksia viestistä (koska kyseessä on simuloitu hyökkäys).

- Raportit: Kun simuloitu hyökkäys on valmis, voit tarkastella raporttia valitsemalla **Hyökkäystiedot.**

- Yksityiskohtaiset ohjeet ja uudet ominaisuudet Attack Simulatorissa ovat [ohjeaiheessa Attack Simulator Microsoft 365:ssä](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
