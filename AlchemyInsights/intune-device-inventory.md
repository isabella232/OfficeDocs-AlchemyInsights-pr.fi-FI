---
title: Intune-laitteen luettelointi
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
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667875"
---
# <a name="intune-device-inventory"></a>Intune-laitteen luettelointi

Laitteet-Blade tarjoaa hallinnoijan käsityksen laitteista, jotka ovat hallinta-kohdassa Intunella laitekohtaisesti. Näytetyt tiedot sisältävät: laitteisto, löydetyt sovellukset, laitteen yhteensopivuus tila ja laitteen määritys tila.

Laitteiston ja löydettyjen sovellusten varasto tiedot kerätään seitsemän päivän jaksolle. Sovellusten ja laitteiden tietyt ominaisuudet on ilmoitettu eri tavalla laitteen käyttö järjestelmän mukaan ja sen mukaan, onko laite henkilökohtaisesti vai yrityksen omistama.

Lisä tietoja on kohdassa [laitteen tietojen tarkasteleminen Intunella](https://docs.microsoft.com/intune/device-inventory).

**Usein kysytyt kysymykset**

K: en saa täyttä luetteloa sovelluksista, jotka esiintyvät Intune-kirjoilla Windows-laitteissa. Miksi ei?

A: tällä hetkellä vain nykyaikaisia sovelluksia on lueteltu Windows 10-tieto koneissa, jotka tunnistetaan yritys laitteiksi. Intune ei kerää tietoja näihin laitteisiin asenne tuista Win32-sovelluksista.

K: Miksi Puhelin numeroita ei ole kerätty kaikista laitteista?

A: Intunen yritys käyttöön luokiteltuja puhelimia ei ole tunnistettu koko Puhelin numeroksi, kun suoritat esimerkiksi mobiililaitteiden inventaario raportin. Tuo sinulle-laitteen Puhelin numerot on aina osittain peitetty tähdellä (* * * *) ja näyttää vain viimeiset neljä numeroa.