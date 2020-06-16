---
title: Omistaja ei voi luoda alikansiota Outlookin avulla
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/12/2020
ms.locfileid: "44748906"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Omistaja ei voi luoda alikansiota Outlookin avulla

**Yleisten kansioiden omistajissa on jatkuva ongelma, joka luo alikansioita Outlookin avulla. Ongelma korjataan pian.**

Käytä samalla jotakin seuraavista kiertotavoista:

1. Outlook for MAC:n avulla voit luoda alikansion, koska ongelma vaikuttaa vain Outlook työpöytäikkunoihin (kaikki versiot)
2. Hankkia admin aiheuttaa subfolder kohteleva EXO Hylsy eli EAC
3. Käyttäjän DefaultPublicFolderMailbox/EffectivePublicFolderMailbox-kansion muuttaminen muuhun postilaatikkoon kuin ongelman aiheuttavan kansion sisältöpostilaatikkoon  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Odota tunti, käynnistä Outlook-asiakasohjelma uudelleen