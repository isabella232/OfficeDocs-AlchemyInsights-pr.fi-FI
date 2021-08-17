---
title: Bitlocker-palautusavaimet
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: f71fae0aabda3fc48f20d5ea1e6909475f0c17ff5cdf98b58b1403bd2e291c19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060061"
---
# <a name="accessing-bitlocker-recovery-keys"></a>BitLocker-palautusavainten käyttäminen

Kun määrität BitLocker-asetuksia Intune Endpoint Protection käytäntöä, on mahdollista määrittää, tallennetaanko BitLocker-palautustiedot Azure Active Directory.

Jos tämä asetus on määritetty, tallennettujen palautustietojen pitäisi näkyä Intune-järjestelmänvalvojalle osana laitteen tietuetietoja Intune-laitteissa kahdella tavalla:

Laitteet - Azure AD -laitteet > "Laite" TAI Laitteet -> Kaikki laitteet -> "Laite" -> palautusavaimet

Jos itse laitteella on järjestelmänvalvojan käyttöoikeudet, palautusavain (salasana) voidaan nähdä suorittamalla seuraava komento järjestelmänvalvojan oikeuksin oikeutetussa komentokehotteessa:

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
Jos laite on salattu ennen intune-salausta, palautusavain on ehkä liitetty Microsoft-tiliin (MSA), jota käytetään laitteeseen kirjautumisessa OOBE-prosessin aikana. Tässä tapauksessa MSA:n käytön ja sisäänkirjautumisen pitäisi näyttää  https://onedrive.live.com/recoverykey laitteet, joiden palautusavaimet on tallennettu.
 
Jos laite on salattu toimialuepohjaisen ryhmäkäytännön tuloksena, palautustiedot saatetaan tallentaa paikalliseen Active Directoryyn.

Jos olet määrittänyt Endpoint-suojauskäytännön, joka tallentaa palautusavaimen Azure Active Directory mutta tietyn laitteen avainta ei ole ladattu, voit käynnistää latauksen kiertämällä palautusavaimen laitteesta MEM-konsolista. Lisätietoja on kohdassa [BitLocker-palautusavainten kiertäminen.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

