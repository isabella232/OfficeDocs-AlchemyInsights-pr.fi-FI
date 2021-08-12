---
title: Kaatumisongelmien OneDrive vianmääritys
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921004"
---
# <a name="troubleshoot-onedrive-crashes"></a>Kaatumisongelmien OneDrive vianmääritys

Jos OneDrive kaatuu toistuvasti, kokeile seuraavia vianmääritysohjeita:

**Varmista, että rekisteriavaimia ei ole määritetty:**

1. Siirry rekisterieditorin avulla HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Jos DisableFileSyncNGSC on käytössä ja sen arvona on 1, avaa avain ja muuta arvoksi 0.
3. Käynnistä OneDrive manuaalisesti valitsemalla Aloitus ![Paina Windows näppäintä](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), OneDrive hakuruutuun ja napsauta sitten OneDrive työpöytäsovellusta.

**Palauta OneDrive:**

Huomautukset:

- Asetusten OneDrive katkaisee kaikki olemassa olevat synkronointiyhteydet (mukaan lukien henkilökohtainen OneDrive jos se on määritetty).
- Tiedostoja tai tietoja ei menetetä palauttamalla OneDrive tietokoneessa.

**Voit palauttaa OneDrive:**

1. Avaa Suorita-valintaikkuna painamalla näppäinyhdistelmää Windows R.
2. Kirjoita %localappdata%\Microsoft\OneDrive\onedrive.exe /reset ja paina OK. Komentoikkuna saattaa tulla näkyviin hetkeksi.
3. Käynnistä OneDrive manuaalisesti valitsemalla Aloitus ![Paina Windows näppäintä](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), OneDrive hakuruutuun ja napsauta sitten OneDrive työpöytäsovellusta.

Huomautukset:

- Jos valitsit vain joidenkin kansioiden synkronoinnin ennen palautusta, sinun on tehtävä se uudelleen, kun synkronointi on valmis. Lisätietoja [on OneDrive, mitkä kansiot haluat](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)synkronoida   tietokoneeseen.
- Sinun on tehtävä tämä henkilökohtaisen työsi OneDrive OneDrive for Business.