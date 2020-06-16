---
title: OneDriven kaatumisiin liittyviä ongelmia
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/15/2020
ms.locfileid: "44748918"
---
# <a name="troubleshoot-onedrive-crashes"></a>OneDriven kaatumisiin liittyviä ongelmia

Jos OneDrive kaatuu toistuvasti, kokeile seuraavia vianmääritysohjeita:

**Varmista, että rekisteriavaimia ei ole määritetty:**

1. Siirry Rekisterieditorin avulla kohtaan HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Jos DisableFileSyncNGSC on olemassa ja sen arvo on 1, avaa avain ja muuta arvoksi 0.
3. Käynnistä OneDrive manuaalisesti käynnistämällä aloitus ![Paina Windows-näppäintä](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), kirjoita hakuruutuun OneDrive ja napsauta sitten OneDrive-työpöytäsovellusta.

**Nollaa OneDrive:**

Muistiinpanoja:

- OneDriven nollaaminen katkaisee kaikki nykyiset synkronointiyhteytesi (mukaan lukien henkilökohtaisen OneDriven, jos se on määritetty).
- Et menetä tiedostoja tai tietoja palauttamalla OneDriven tietokoneeseen.

**OneDriven nollaaminen:**

1. Avaa Suorita-valintaikkuna painamalla Windows-näppäintä ja R-näppäintä.
2. Kirjoita %localappdata%\Microsoft\OneDrive\onedrive.exe /reset ja paina OK-painiketta. Komentoikkuna saattaa näkyä lyhyesti.
3. Käynnistä OneDrive manuaalisesti käynnistämällä aloitus ![Paina Windows-näppäintä](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), kirjoita hakuruutuun OneDrive ja napsauta sitten OneDrive-työpöytäsovellusta.

Muistiinpanoja:

- Jos olet valinnut vain joidenkin kansioiden synkronoinnin ennen nollausta, sinun on tehtävä se uudelleen, kun synkronointi on valmis. Lisätietoja on kohdassa [Tietokoneeseen synkronoitavien OneDrive-kansioiden](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   valitseminen.
- Sinun on suoritettava tämä henkilökohtaiseen OneDriveen ja OneDrive for Businessiin.