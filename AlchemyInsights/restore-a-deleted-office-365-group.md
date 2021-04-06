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
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597440"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Poistetun Microsoft 365 -ryhmän palauttaminen

Voit palauttaa poistetun Microsoft 365 -ryhmän tai Microsoft Teamsin 30 päivän kuluessa poistamisesta.

1. Siirry [Microsoft 365 -hallintakeskukseen ja kirjaudu](https://aka.ms/RestoreDeletedGroup) sisään ja luetella poistetut ryhmät ja tiimit.

    **Huomautus:** Kirjaudu sisään käyttämällä tiliä, joka on määritetty joko vuokraajan järjestelmänvalvojalle tai ryhmien järjestelmänvalvojan roolille.

1. Valitse poistettu Microsoft 365 -ryhmä/Teams palautettavaksi ja valitse **Palauta ryhmä**.

    Jos ryhmää ei voi palauttaa ristiriitaisten SMTP-osoitteiden vuoksi, etsi ristiriitaa aiheuttava objekti seuraavan komennon avulla ja poista SMTP-osoite:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Huomautus:** Joissakin tapauksissa voi kestää jopa 24 tuntia, ennen kuin ryhmä ja kaikki sen tiedot palautetaan.

    Lisätietoja tai lisätietoja ryhmien palauttamisesta PowerShellin avulla on kohdassa [Poistetun Microsoft 365 -ryhmän palauttaminen.](https://go.microsoft.com/fwlink/?linkid=867802)