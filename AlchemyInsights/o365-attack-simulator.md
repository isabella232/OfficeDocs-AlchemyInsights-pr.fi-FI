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
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801548"
---
# <a name="attack-simulator-in-microsoft-365"></a>Hyökkäys simulaattori Microsoft 365-sovelluksessa

- Oletko puuttuvasta hyökkäys simulaattorista? Hyökkäys simulaattori edellyttää **Microsoft Defender for office 365-ohjelmaa (ATP-sopimus 2)** tai **Office 365 Enterprise-E5** . Hyökkäys simulaattori ei **sisälly Microsoft** Defender for Office 365-pakettiin (ATP-Paketti 1), Office 365 Enterprise E3-ohjelmaan tai mihinkään Microsoft 365-sovellukseen yritys tilauksia varten.

- Tili, jota käytät simuloitujen hyökkäysten käynnistämiseen, edellyttää yleisten järjestelmänvalvojien tai suojaus järjestelmänvalvojien käyttö oikeuksia ja usean tekijän todennusta. Lisä tietoja hyökkäys simulaattori vaatimuksista on [tässä](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)artikkelissa.

- Tärkeitä huomioitavia asioita **Brute Force-Sala sanan** hyökkäys simulaatioista:

  - Jos kohde tilillä on käytössä MFA ja sala sana on oikein, tili ei näy vaarantuneen (toinen todennus kerroin on epätäydellinen).

  - Salasana tiedosto ei voi olla suurempi kuin 10 Mt. Käytä yhtä riviä kohden Sala sanaa ja Sisällytä tyhjä rivi (rivin vaihto) luettelon viimeisen Sala sanan perään.

- Tärkeitä asioita, jotka on hyvä tietää **Spear phishing** Liitä-simulaatioista:

  - Et voi määrittää mukautettua arvoa **tietojen kalastelu-kirjautumispalvelimen URL-osoitteille** .

  - Jos vastaanottajalla on käytössä [Ilmoita viestistä-apuohjelma](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , joka ilmoittaa viestin tietojenkalasteluksi, et ehkä saa ilmoituksia viestistä (koska kyseessä on simuloitu hyökkäys).

- Raportit: kun simuloitu hyökkäys on valmis, voit tarkastella raporttia napsauttamalla **hyökkäys tiedot** -painiketta.

- Yksityiskohtaisia ohjeita ja hyökkäys simulaattorin uusia ominaisuuksia on artikkelissa [hyökkäys simulaattori Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)-sovelluksessa.
