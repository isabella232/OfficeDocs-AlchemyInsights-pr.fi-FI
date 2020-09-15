---
title: BitLocker-palautus avaimet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685883"
---
# <a name="accessing-bitlocker-recovery-keys"></a>BitLocker-palautus avainten käyttäminen

Kun määrität BitLocker-asetukset Intune-pääte pisteen suojaus käytännöksi, on mahdollista määrittää, tallennetaanko BitLocker-palautus tiedot Azure Active Directoryyn.

Jos tämä asetus on määritetty, tallennettujen palautus tietojen pitäisi näkyä Intune-järjestelmänvalvojalle osana laitteen tietue tietoja Intune-laitteiden Blade-sovelluksessa kahdella tavalla:

Laitteet-Azure AD Devices-> "laite" tai laitteet-> kaikki laitteet-> "laite"-> palautus näppäimet

Jos itse laitteessa on järjestelmänvalvojan oikeudet, palautus avain (sala sana) näkyy suorittamalla seuraava komento järjestelmänvalvojan oikeuksin suoritettavalla komento kehotteesta:

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
Jos laite on salattu ennen sen rekisteröimisestä Intune-avaimeen, palautus avain on ehkä liitetty "Microsoft-tiliin" (MSA), jota käytettiin laitteeseen kirjautumiseen OOBE-prosessin aikana. Tässä tapa uksessa  https://onedrive.live.com/recoverykey tämän MSA-palvelun käyttö ja sisäänkirjautuminen olisi osoitettava laitteet, joihin palautus avaimet on tallennettu.
 
Jos laite on salattu kokoonpanon perusteella toimi alue perusteista ryhmä käytäntöä käyttämällä, palautus tiedot saatetaan tallentaa paikalliseen Active Directoryyn.
 

