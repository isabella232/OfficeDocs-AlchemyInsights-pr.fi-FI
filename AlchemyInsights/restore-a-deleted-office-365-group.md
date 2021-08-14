---
title: Poistetun ryhmän Microsoft 365 palauttaminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959023"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Poistetun ryhmän Microsoft 365 palauttaminen

Voit palauttaa poistetun Microsoft 365 ryhmän tai Microsoft Teams 30 päivän kuluessa poistamisesta.

1. Siirry [Microsoft 365 -hallintakeskus](https://aka.ms/RestoreDeletedGroup) luetteloon, jossa olet poistetut ryhmät ja tiimit.

    **Huomautus:** Kirjaudu sisään käyttämällä tiliä, joka on määritetty joko vuokraajan järjestelmänvalvojalle tai ryhmien järjestelmänvalvojan roolille.

1. Valitse poistetut Microsoft 365 tai Teams palautettava ryhmä ja valitse **Palauta ryhmä**.

    Jos ryhmää ei voi palauttaa ristiriitaisten SMTP-osoitteiden vuoksi, etsi ristiriitaa aiheuttava objekti seuraavan komennon avulla ja poista SMTP-osoite:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Huomautus:** Joissakin tapauksissa voi kestää jopa 24 tuntia, ennen kuin ryhmä ja kaikki sen tiedot palautetaan.

    Lisätietoja tai lisätietoja ryhmien palauttamisesta PowerShellin avulla on kohdassa Poistetun ryhmän [Microsoft 365 palauttaminen.](https://go.microsoft.com/fwlink/?linkid=867802)