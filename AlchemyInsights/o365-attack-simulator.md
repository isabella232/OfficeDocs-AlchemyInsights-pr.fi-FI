---
title: 2681 hyökkäys simulaattori Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305329"
---
# <a name="attack-simulator-in-office-365"></a>Hyökkäys simulaattori Office 365

- Puuttuuko hyökkäys simulaattori? Hyökkäys simulaattori edellyttää **office 365 Advanced uhkien torjunta suunnitelma 2 (ATP-suunnitelma 2)** tai **Office 365 Enterprise E5**. Hyökkäys simulaattori **ei** sisälly Office 365 Advanced Threat Protection-suunnitelmaan 1 (ATP-suunnitelma 1), Office 365 Enterprise E3-yritykseen tai mihin tahansa Office 365-yritys tilauksiin.

- Simuloitujen hyökkäysten käynnistämiseen käytettävä tili edellyttää yleisen järjestelmänvalvojan tai suoja uksen järjestelmänvalvojan oikeuksia ja monimitostodennusta (MFA). Lisä tietoja hyökkäys simulaattorin vaatimuksista [on tässä ohje aiheessa](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Tärkeitä asioita tietää **Brute Force sala sana** hyökkäys simulaatiot:

  - Jos kohde tili on MFA käytössä ja sala sana on arvattu oikein, tiliä ei näy vaarantuneeksi (toinen todennus kerroin on puutteellinen).

  - Salasana tiedoston koko ei voi olla suurempi kuin 10 Mt. Käytä yksi sala sana riviä kohden ja Sisällytä tyhjä rivi (rivin tuotto) luettelon viimeisen Sala sanan jälkeen.

- Tärkeitä asioita tietää **Spear phishing** Liitä simulaatiot:

  - Et voi antaa mukautettua arvoa **tietojen kalastelun torjunta palvelimen URL-osoitteelle**.

  - Jos vastaanottaja ilmoittaa sanoman tietojenkalasteluksi [Ota käyttöön raportti viesti-apuohjelman](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) avulla, et ehkä saa ilmoituksia viestistä (koska kyseessä on simuloitu hyökkäys).

- Raportit: kun simuloitu hyökkäys on valmis, voit napsauttaa **hyökkäys tiedot** nähdäksesi raportin.

- Tarkempia ohjeita ja uusia ominaisuuksia hyökkäys simulaattori, katso [hyökkäys simulaattori Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
