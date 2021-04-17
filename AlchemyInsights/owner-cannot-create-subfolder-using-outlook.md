---
title: Omistaja ei voi luoda alikansiota Outlookin avulla
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836132"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Omistaja ei voi luoda alikansiota Outlookin avulla

**Alikansioiden luomisessa Outlookissa on meneillään ongelma, jossa yleisen kansion omistajat luovat alikansioita. Ongelma korjataan pian.**

Sillä välin voit käyttää yhtä seuraavista vaihtoehtoista tavoista:

1. Käytä Outlook for MACia alikansion luomiseen, koska ongelma vaikuttaa vain Outlookin työpöytäversioihin (kaikki versiot)
2. Järjestelmänvalvojan on luotava alikansio EXO Shellin tai EAC:n avulla
3. Käyttäjän DefaultPublicFolderMailbox/EffectivePublicFolderMailbox-kansion muuttaminen muuhun kuin kansion sisältöpostilaatikkoon, joka aiheuttaa ongelman  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Odota tunti, käynnistä Outlook-asiakasohjelma uudelleen