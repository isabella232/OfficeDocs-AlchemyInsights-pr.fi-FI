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
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505683"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Poistetun Microsoft 365 -ryhmän palauttaminen

Voit palauttaa poistetun Microsoft 365 -ryhmän tai Microsoft Teamsin 30 päivän kuluessa poistamisesta.

1. Jos haluat kirjautua Microsoft 365 -hallintakeskukseen ja luetella poistetut ryhmät ja ryhmät, siirry [Microsoft 365 -hallintakeskukseen.](https://aka.ms/RestoreDeletedGroup)

    **Huomautus:** Kirjaudu sisään käyttämällä tiliä, joka on määritetty joko vuokraajan järjestelmänvalvojalle tai ryhmien järjestelmänvalvojan roolille.

1. Valitse palautettava poistettu Microsoft 365 -ryhmä tai Teams ja valitse **palauta ryhmä.**

    Jos ryhmää ei voi palauttaa ristiriitaisten SMTP-osoitteiden vuoksi, etsi ristiriitaa aiheuttava objekti seuraavan komennon avulla ja poista SMTP-osoite:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Huomautus:** Joissakin tapauksissa voi kestää jopa 24 tuntia, ennen kuin ryhmä ja kaikki sen tiedot palautetaan.

    Lisätietoja tai tietoja ryhmien palauttamisesta PowerShellin avulla on ohjeaiheessa [Poistetun Microsoft 365 -ryhmän palauttaminen.](https://go.microsoft.com/fwlink/?linkid=867802)