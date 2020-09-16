---
title: 2681-hyökkäys simulaattori Microsoft 365-sovelluksessa
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759216"
---
# <a name="attack-simulator-in-microsoft-365"></a>Hyökkäys simulaattori Microsoft 365-sovelluksessa

- Oletko puuttuvasta hyökkäys simulaattorista? Hyökkäys simulaattori edellyttää **office 365 Advanced Threat Protectionin 2-ohjelmaa (ATP-sopimus 2)** tai **Office 365 Enterprise-E5**. Hyökkäys simulaattori **ei** sisälly Office 365 Advanced Threat PROTECTIONIN (ATP-Paketti 1), Office 365 Enterprise E3-ohjelmaan tai mihinkään Microsoft 365-sovellukseen yritys tilauksia varten.

- Tili, jota käytät simuloitujen hyökkäysten käynnistämiseen, edellyttää yleisten järjestelmänvalvojien tai suojaus järjestelmänvalvojien käyttö oikeuksia ja usean tekijän todennusta. Lisä tietoja hyökkäys simulaattori vaatimuksista on [tässä](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)artikkelissa.

- Tärkeitä huomioitavia asioita **Brute Force-Sala sanan** hyökkäys simulaatioista:

  - Jos kohde tilillä on käytössä MFA ja sala sana on oikein, tili ei näy vaarantuneen (toinen todennus kerroin on epätäydellinen).

  - Salasana tiedosto ei voi olla suurempi kuin 10 Mt. Käytä yhtä riviä kohden Sala sanaa ja Sisällytä tyhjä rivi (rivin vaihto) luettelon viimeisen Sala sanan perään.

- Tärkeitä asioita, jotka on hyvä tietää **Spear phishing** Liitä-simulaatioista:

  - Et voi määrittää mukautettua arvoa **tietojen kalastelu-kirjautumispalvelimen URL-osoitteille**.

  - Jos vastaanottajalla on käytössä [Ilmoita viestistä-apuohjelma](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , joka ilmoittaa viestin tietojenkalasteluksi, et ehkä saa ilmoituksia viestistä (koska kyseessä on simuloitu hyökkäys).

- Raportit: kun simuloitu hyökkäys on valmis, voit tarkastella raporttia napsauttamalla **hyökkäys tiedot** -painiketta.

- Yksityiskohtaisia ohjeita ja hyökkäys simulaattorin uusia ominaisuuksia on artikkelissa [hyökkäys simulaattori Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)-sovelluksessa.
