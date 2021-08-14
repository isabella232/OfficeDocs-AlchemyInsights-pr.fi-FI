---
title: Omistaja ei voi luoda alikansiota Outlook
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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063121"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Omistaja ei voi luoda alikansiota Outlook

**Alikansioita luovien julkisten kansioiden omistajien käytössä on jatkuva ongelma Outlook. Ongelma korjataan pian.**

Sillä välin voit käyttää yhtä seuraavista vaihtoehtoista tavoista:

1. Käytä Outlook for Macia alikansion luomiseen, sillä ongelma vaikuttaa vain Outlook työpöytäikkunoihin (kaikki versiot)
2. Järjestelmänvalvojan on luotava alikansio EXO Shellin tai EAC:n avulla
3. Käyttäjän DefaultPublicFolderMailbox/EffectivePublicFolderMailbox-kansion muuttaminen muuhun kuin kansion sisältöpostilaatikkoon, joka aiheuttaa ongelman  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Odota tunti, käynnistä Outlook-asiakasohjelma uudelleen