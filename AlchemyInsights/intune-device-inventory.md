---
title: Intune Device Inventory
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 00ee4f1d7130c239272e28ee8e051a18e6e0baf13040d2a892866be5900adfaf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014069"
---
# <a name="intune-device-inventory"></a>Intune Device Inventory

Laitteet-teristä saat järjestelmänvalvojan tiedot Intunen hallinnassa olelluista laitteista laitekohtaisesti. Näkyvissä ovat seuraavat tiedot: Laitteisto, Löydetyt sovellukset, Laitteen yhteensopivuustila ja Laitteen määritykset -tila.

Laitteiston ja löydettyjen sovellusten varastotiedot kerätään seitsemän päivän jaksolla. Raportoidut sovellukset ja laitekohtaiset elementit vaihtelevat laitteen käyttöjärjestelmän mukaan ja sen mukaan, onko laite henkilökohtainen vai yrityksen omistama.

Lisätietoja on kohdassa Laitteen [tietojen katsominen Intunessa.](https://docs.microsoft.com/intune/device-inventory)

**Usein kysytyt kysymykset**

K: En saa täyttä sovellusluetteloa Intune-rekisteröityjen sovellusten Windows laitteista. Miksi ei?

A: Tällä hetkellä vain nykyaikaiset sovellukset on lueteltu Windows 10 tietokoneissa, jotka on tunnistettu yrityksen laitteisiin. Intune ei kerää tietoja näihin laitteisiin asennetuista Win32-sovelluksista.

K: Miksi puhelinnumeroita ei kerätä kaikista laitteista?

A: Intunessa yrityksen laitteisiin luokiteltuja puhelimia ei tunnisteta niiden koko puhelinnumerolla esimerkiksi silloin, kun suoritat mobiililaitevarastoraportin. Tuo oman laitteen puhelinnumerot on aina osittain peitetty tähdellä (****) ja näytetään vain neljä viimeistä numeroa.