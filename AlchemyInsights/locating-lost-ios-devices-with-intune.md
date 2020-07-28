---
title: Kadonneiden iOS-laitteiden etsiminen Intunen avulla
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
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439625"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Kadonneiden iOS-laitteiden etsiminen Intunen avulla

Kun kadonnut tila otetaan käyttöön iOS-laitteessa, järjestelmänvalvoja voi näyttää lukitusnäytössä viestin ja puhelinnumeron.

Kun kadonnut tila on käytössä, järjestelmänvalvoja voi paikantaa laitteen paikannuksen avulla laitteen fyysisen sijainnin.

Intunen Paikanna laite -toiminto toimii iOS-laitteiden kanssa näyttääkseen tietyn laitteen sijainnin kartalla.

Tämän toiminnon käyttäminen edellyttää, että iOS-laite on:

- Valvottu tila
- Kadonnut-tila

Lisätietoja on ohjeissa [Kadonneen tilan ottaminen käyttöön iOS/iPadOS-laitteissa, joissa on Intune](https://docs.microsoft.com/intune/device-lost-mode) ja [Etsi kadonneet tai varastetut iOS/iPadOS-laitteet Intunella](https://docs.microsoft.com/intune/device-locate).

**Usein kysytyt kysymykset**

K: Tein etätoiminnon yrityksen tietojen poistamiseksi laitteesta, ja nyt se on jumissa odottavassa tilassa.

: Jotta etätoiminto onnistuisi, kohdelaitteen on oltava online-tilassa ja terve. Seuraavissa tilanteissa etätoiminto pysyy odottavassa tilassa 30 päivän ajan tai kunnes laite hyväksyy komennon:

- Jos laitteessa ei ole yhteyttä
- Kun laite menettää hallintatilansa Intune

Jos epäilet, että laite ei enää kirjaudu sisään ja että se ei voi poistaa yrityksen tietoja, valitse Poista. Poistaminen poistaa laitetietueen niin, että se ei enää näy Intune-laiteluettelossa. Jos laite aktivoituu uudelleen, sen käyttäjän on rekisteröitävä se uudelleen.

K: Miksi tietyt etätoiminnot eivät ole käytettävissä?

A: Kaikki alustat eivät tue kaikkia etälaitetoimintoja. Seuraavat etätoiminnot ovat alustakohtaisia, joten ne ovat käytettävissä vain mainittujen alustojen osalta.

- Ohita aktivointilukitus (vain iOS)
- Tuore käynnistys (vain Windows)
- Kadonnut-tila (vain iOS)
- Laitteen paikantaminen (vain iOS)
- Käynnistä uudelleen (vain Windows)

Lisätietoja kustakin toiminnosta on kohdassa [Käytettävissä olevat laitetoiminnot](https://docs.microsoft.com/intune/device-management#available-device-actions).