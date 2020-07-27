---
title: Ohita aktivointilukitus valvotuissa iOS-laitteissa Intunen avulla
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423735"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Ohita aktivointilukitus valvotuissa iOS-laitteissa Intunen avulla

IOS-laitteiden aktivointilukituksen ohittaminen helpottaa toipumista skenaariosta, jossa käyttäjä ottaa käyttöön aktivointilukituksen yrityslaitteessa ja poistuu sitten yrityksestä.

Aktivointilukon ohittamisen edellytyksenä ovat seuraavat:

- Laite on "valvottu".
- Aktivointilukitus on otettu käyttöön iOS-laiterajoituskäytännön avulla Intuessa.

Lisäksi aktivointilukon ohitettaessa sinun on

- Fyysisesti hallussaan laite pyyhitään.
- Kopioi koodi ennen pyyhkimisen antamista.

**Huomautus:** Pyyhikoodissa isot ja pienet kirjaimet eivät ole isot ja pienet kirjaimet, joten "-"-merkkejä ei tarvita.

Lisätietoja on kohdassa [Aktivointilukituksen ohitttaminen valvotuissa iOS-laitteissa Intune -toiminnolla](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**Usein kysytyt kysymykset**

K: **Tein etätoiminnon yrityksen tietojen poistamiseksi laitteesta, ja nyt se on jumissa odottavassa tilassa.**

: Jotta etätoiminto onnistuisi, kohdelaitteen on oltava online-tilassa ja terve. Seuraavissa tilanteissa etätoiminto pysyy odottavassa tilassa 30 päivän ajan tai kunnes laite hyväksyy komennon, kun laite:

- Ei ole yhteyttä.
- Menettää johdon tilan Intunella.

Jos epäilet, että laite ei enää kirjaudu sisään ja että se ei poista yrityksen tietoja, valitse Poista. Poistaminen poistaa laitetietueen niin, että se ei enää näy Intune-laiteluettelossa. Jotta laite aktivoituu uudelleen, sen käyttäjän on rekisteröitävä laite uudelleen.

K: **Miksi tietyt etätoiminnot eivät ole käytettävissä?**

A: Kaikki alustat eivät tue kaikkia etälaitetoimintoja. Seuraavat etätoiminnot ovat ympäristökohtaisia.

- Ohita aktivointilukitus (vain iOS)
- Tuore käynnistys (vain Windows)
- Kadonnut-tila (vain iOS)
- Laitteen paikantaminen (vain iOS)
- Käynnistä uudelleen (vain Windows)

Lisätietoja kustakin toiminnosta on kohdassa [Käytettävissä olevat laitetoiminnot](https://docs.microsoft.com/intune/device-management#available-device-actions).