---
title: OneDrive-kaatumisten vian määritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664995"
---
# <a name="troubleshoot-onedrive-crashes"></a>OneDrive-kaatumisten vian määritys

Jos OneDrive kaatuu toistuvasti, kokeile seuraavia vian määritys ohjeita:

**Varmista, että rekisteri avaimia ei ole valittu:**

1. Kun käytät rekisteri editoria, siirry kohtaan HKEY_LOCAL_MACHINE \Software\policiesmicrosoft\onedrive
2. Jos Disasemfilesyncpääsihteeristön arvo on 1, Avaa avain ja muuta arvoksi 0.
3. Käynnistä OneDrive manuaalisesti käynnistämällä ![Paina Windows-näppäintä](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), kirjoita haku ruutuun OneDrive ja valitse sitten OneDrive-Työpöytä sovellus.

**Palauta OneDrive:**

Toteaa

- OneDriven palauttaminen katkaisee kaikki olemassa olevat synkronointi yhteydet (mukaan lukien henkilökohtainen OneDrive, jos se on määritetty).
- Tiedostoja tai tietoja ei menetetä palauttamalla OneDrive tieto koneeseen.

**OneDriven palauttaminen:**

1. Avaa Suorita-valinta ikkuna painamalla näppäin yhdistelmää Windows-näppäintä ja R.
2. Kirjoita% localappdata% \Microsoft\OneDrive\onedrive.exe/reset ja paina OK. Komento ikkuna voi näkyä lyhyesti.
3. Käynnistä OneDrive manuaalisesti käynnistämällä ![Paina Windows-näppäintä](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), kirjoita haku ruutuun OneDrive ja valitse sitten OneDrive-Työpöytä sovellus.

Toteaa

- Jos olet valinnut vain joidenkin kansioiden synkronoinnin ennen palauttamista, sinun on tehtävä se uudelleen, kun synkronointi on valmis. Lue lisä tietoja artikkelista [Valitse, mitkä OneDrive-kansiot synkronoidaan tieto koneeseen](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   .
- Sinun on suoritettava tämä henkilökohtaiseen OneDrive-ja OneDrive for Business-palveluun.