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
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820283"
---
# <a name="accessing-bitlocker-recovery-keys"></a>BitLocker-palautusavainten käyttäminen

Kun määrität BitLocker-asetuksia Intune Endpoint Protection Policy -palvelussa, on mahdollista määrittää, tallennetaanko Bitlocker-palautustiedot Azure Active Directoryyn.

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

Jos olet määrittänyt Endpoint-suojauskäytännön, joka tallentaa palautusavaimen Azure Active Directoryyn, mutta tietyn laitteen avainta ei ole ladattu, voit käynnistää latauksen kiertämällä palautusavaimen laitteesta MEM-konsolista. Lisätietoja on kohdassa [BitLocker-palautusavainten kiertäminen.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

