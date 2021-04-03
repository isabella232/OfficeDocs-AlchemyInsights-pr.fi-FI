---
title: Bitlocker-palautusavaimet
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
ms.openlocfilehash: 8708ed76f6abe81582823c8af89db8fffef9a3c5
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505065"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Bitlocker-palautusavainten käyttäminen

Kun määrität Bitlocker-asetuksia Intune Endpoint Protection Policy -palvelussa, on mahdollista määrittää, tallennetaanko Bitlocker-palautustiedot Azure Active Directoryyn.

Jos tämä asetus on määritetty, tallennettujen palautustietojen pitäisi näkyä Intune-järjestelmänvalvojalle osana laitteen tietojen tallennusta Intune Devices -laitteissa kahdella tavalla:

Laitteet - Azure AD -laitteet > "Laite" tai laitteet -> Kaikki laitteet -> "Laite" -> palautusavaimet

Jos itse laitteessa on järjestelmänvalvojan käyttöoikeudet, palautusavain (salasana) näkyy suorittamalla seuraava komento järjestelmänvalvojan oikeuksin hallittavasta komentokehotteesta:

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
Jos laite on salattu ennen intune-kirjautumista, palautusavain on ehkä liitetty Microsoft-tiliin (MSA), jota käytetään kirjautumiseen laitteeseen OOBE-prosessin aikana. Jos näin oli, MSA:n käytön ja sisäänkirjautumisen pitäisi näyttää laitteet,  https://onedrive.live.com/recoverykey joille palautusavaimet on tallennettu.
 
Jos laite on salattu toimialuepohjaisen ryhmäkäytännön perusteella, palautustiedot saatetaan tallentaa paikalliseen Active Directoryyn.

Jos olet määrittänyt Endpoint-suojauskäytännön, joka tallentaa palautusavaimen Azure Active Directoryyn, mutta tietyn laitteen avainta ei ole ladattu, voit käynnistää latauksen kiertämällä laitteen palautusavainta MEM-konsolista. Lisätietoja on kohdassa [BitLocker-palautusavainten kiertäminen.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

