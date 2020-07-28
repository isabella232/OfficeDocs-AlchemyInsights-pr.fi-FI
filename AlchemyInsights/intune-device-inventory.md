---
title: Intune Laitteen varasto
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439653"
---
# <a name="intune-device-inventory"></a>Intune Laitteen varasto

Laitteet-terä antaa järjestelmänvalvojan käsityksen Intunen hallinnassa olevista laitteista laitekohtaisesti. Näytettyjä tietoja ovat: Laitteisto, Löydetyt sovellukset, Laitevaatimustenmukaisuuden tila ja Laiteasetukset-tila.

Laitteiston ja löydettyjen sovellusten varastotiedot kerätään seitsemän päivän jakson aikana. Raportoidut sovellukset ja laitteiston erityiselementit vaihtelevat laitteen käyttöjärjestelmän ja sen mukaan, onko laite henkilökohtaisesti vai yrityksen omistuksessa.

Lisätietoja on kohdassa [Laitteen tiedot kohdassa Intune](https://docs.microsoft.com/intune/device-inventory).

**Usein kysytyt kysymykset**

K: En saa täydellistä luetteloa Intune-rekisteröimistä Windows-laitteista olevista sovelluksista. Miksi ei?

: Tällä hetkellä vain nykyaikaiset sovellukset on lueteltu Windows 10 -tietokoneissa, jotka on tunnistettu yrityslaitteisiksi. Intune ei kerää tietoja näihin laitteisiin asennetuista Win32-sovelluksista.

K: Miksi puhelinnumeroita ei kerätä kaikista laitteista?

: Intunen yrityssiitoittereiksi luokiteltuja puhelimia ei tunnisteta täydellä puhelinnumerolla, kun esimerkiksi suoritat mobiililaitteen inventaarioraportin. Tuo sinulle oma-laite puhelinnumerot peitetään aina osittain tähtillä (****), ja niissä näkyvät vain neljä viimeistä numeroa.