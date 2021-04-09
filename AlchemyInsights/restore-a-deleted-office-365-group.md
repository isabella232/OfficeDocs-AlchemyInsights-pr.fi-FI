---
title: Poistetun Microsoft 365 -ryhmän palauttaminen
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
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645128"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Poistetun Microsoft 365 -ryhmän palauttaminen

Voit palauttaa poistetun Microsoft 365 -ryhmän tai Microsoft Teamsin 30 päivän kuluessa poistamisesta.

1. Siirry [Microsoft 365 -hallintakeskukseen](https://aka.ms/RestoreDeletedGroup) ja kirjaudu sisään luetteloon, jossa näet, että olet poistetut ryhmät ja tiimit.

    **Huomautus:** Kirjaudu sisään käyttämällä tiliä, joka on määritetty joko vuokraajan järjestelmänvalvojalle tai ryhmien järjestelmänvalvojan roolille.

1. Valitse poistettu Microsoft 365 -ryhmä/Teams palautettavaksi ja valitse **Palauta ryhmä**.

    Jos ryhmää ei voi palauttaa ristiriitaisten SMTP-osoitteiden vuoksi, etsi ristiriitaa aiheuttava objekti seuraavan komennon avulla ja poista SMTP-osoite:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Huomautus:** Joissakin tapauksissa voi kestää jopa 24 tuntia, ennen kuin ryhmä ja kaikki sen tiedot palautetaan.

    Lisätietoja tai lisätietoja ryhmien palauttamisesta PowerShellin avulla on kohdassa [Poistetun Microsoft 365 -ryhmän palauttaminen.](https://go.microsoft.com/fwlink/?linkid=867802)