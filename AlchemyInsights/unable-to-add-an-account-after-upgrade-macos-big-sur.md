---
title: Tiliä ei voi lisätä macOS 11.6 Big Sur -päivityksen jälkeen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506477"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>Tiliä ei voi lisätä macOS 11.6 Big Sur -päivityksen jälkeen

Kun olet päivittämässä macOS 11.6:en, OneDrive:n työ- tai koulutili tai OneDrive-tilisi ei ehkä näy tililuettelossasi sovelluksesta kirjautumalla toiseen tiliin.

Tähän ongelmaan on kehitetty korjaus. Selvitä ensin, onko käytössäsi sovelluksen erillinen versio vai OneDrive:

- Valitse OneDrive pilvestä valikkorivillä ja valitse > **& Asetukset**  >  **Tietoja**  >  **.** Jos versionumero ei sisällä **(erillinen)**-versiota, sinulla on tuotteen App Store -versio.

Jos käytössäsi on erillinen OneDrive, käynnistä tietokone uudelleen ja OneDrive päivitykset koontiversioon, jossa tämä ongelma on ratkaistu. Jos haluat asentaa koontiversion manuaalisesti, lataa [tämä.zip-tiedosto](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip), pura tiedosto ja kopioi OneDrive-sovellus Sovellukset-kansioon (korvaamalla olemassa oleva OneDrive-sovellus).

Jos käytössäsi on App Store -versio, voit asentaa OneDrive. Tämä versio toimii samalla tavalla kuin App Store -versio, mutta sallii Microsoftin tarjota päivityksiä käyttäjille nopeammin ja yhdistää ne versioon, joka sisältää tämän ongelman korjauksen.

1. Lataa korjauksen [OneDrive, joka sisältää korjauksen.](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)
2. Pura tiedosto ja kopioi OneDrive sovellus Sovellukset-kansioon (korvaamalla olemassa oleva OneDrive).

Jos sinun on käytettävä App Store -versiota, odota, että App Store julkaisee sovelluksen version, joka sisältää korjauksen. Valitettavasti Microsoft ei voi ilmoittaa arvioidusta päivämäärästä, jolloin korjattu versio julkaistaan App Storesta.


