---
title: Applen MDM Push -varmennetta ei ole määritetty
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439384"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Applen MDM Push -varmennetta ei ole määritetty

Applen MDM Push Certificate -varmennetta (tunnetaan myös nimellä Applen push-ilmoituspalvelu (APNS) -varmennetta) ei ole määritetty tilaukseesi. Ilman Applen MDM Push Certificate -sertifikaattia et voi rekisteröidä ja hallita iOS- ja Mac OS -laitteita. Kun olet lisännyt varmenteen Intuneen, käyttäjät voivat rekisteröidä iOS-laitteensa asentamalla Yritysportaali-sovelluksen.

1. Valitse **"Olen samaa mieltä".** antaa Microsoftille lupa lähettää tietoja Applelle.

2. Valitse **Lataa csr** Intune-varmenteen allekirjoituspyyntö, joka tarvitaan Applen MDM-push-varmenteen luomiseen. Tiedoston avulla pyydetään luottamussuhdevarmennetta Applen push-varmenteiden portaalista.

3. Siirry Applen push-varmenteiden portaaliin valitsemalla **Luo MDM-push-varmenne.** Kirjaudu sisään yrityksen Apple ID:llä ja valitse luo **varmenne**. Valitse **Valitse tiedosto**, siirry varmenteen allekirjoituspyyntötiedoston kohtaan ja valitse sitten **Lataa**. Lataa varmennetiedosto (.pem) valitsemalla Vahvistus-sivulla **Lataa** ja tallenna tiedosto paikallisesti.
 
**Huomautus:** Varmenne liittyy sen luomiseen käytettyyn Apple ID:hen. Käytä parhaana käytäntönä yrityksen Apple ID:tä hallintatehtäviin ja varmista, että postilaatikkoa valvoo useampi kuin yksi henkilö tai jakeluluetteloa. Älä koskaan käytä henkilökohtaista Apple ID:tä. Käytä samaa Apple ID:tä Apple Push -varmenteen uusimiseen 12 kuukauden välein.
 
4. Anna Apple ID, jota käytetään Applen MDM-push-varmenteen luomiseen. Tallenna tämä tunnus muistutuksena, kun varmenne on uusittava.

5. Siirry varmennetiedostoon (.pem), valitse **Avaa**ja valitse sitten **Lataa**. Push-varmenteella Intune voi rekisteröidä ja hallita Apple-laitteita.