---
title: BitLocker-palautus avaimet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908812"
---
# <a name="accessing-bitlocker-recovery-keys"></a>BitLocker-palautus avainten käyttäminen

Kun määrität BitLocker-asetuksia Intune-pääte pisteen suojaus käytännölle, on mahdollista määrittää, tallennetaanko BitLocker-palautus tiedot Azure Active Directoryyn.

Jos tämä asetus on määritetty, tallennettujen palautus tietojen tulee näkyä Intune Adminissa osana Intune Devices Blade-laitteen tietue dataa kahdella tavalla:

Laitteet-Azure AD Devices-> "laite" tai laitteet-> kaikki laitteet-> "laite"-> palautus avaimet

Vaihtoehtoisesti, jos sinulla on järjestelmänvalvojan oikeudet itse laitteeseen, palautus avain (sala sana) voidaan nähdä suorittamalla seuraava komento järjestelmänvalvojan oikeuksin suoritettavaan komento kehotteeseen:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Jos laite on salattu ennen ilmoittautumista Intunessa, palautus avain on saatettu liittää "Microsoft Account" (MSA)-tiliin, jota käytetään kirjautumiseen laitteeseen OOBE-prosessin aikana. Jos näin oli, yhteyden otto https://onedrive.live.com/recoverykey ja kirjautuminen kyseiseen MSA-tieto koneeseen olisi osoitettava laitteet, joihin palautus avaimet on tallennettu.
 
Jos laite on salattu kokoonpanon seura uksena toimi alueeseen perustuvan ryhmä käytännön kautta, palautus tiedot voidaan tallentaa paikalliseen Active Directoryyn.
 

