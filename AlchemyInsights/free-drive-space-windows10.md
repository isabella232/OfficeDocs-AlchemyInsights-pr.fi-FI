---
title: Levytilan säästäminen Windows 10:ssä
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036592"
---
# <a name="free-up-drive-space-in-windows-10"></a>Levytilan säästäminen Windows 10:ssä

Voit vapauttaa levytilaa Windowsissa kahdella eri vaihtoehdolla:

- Vapauttaa levytilaa Windows 10:ssä.
- Voit vapauttaa tilaa Windows 10:n päivityksille ulkoisella tallennuslaitteella.

Jos levytila on edelleen vähissä levyn uudelleenjärjestämisen käytön jälkeen, tilapäiskansio voi täyttää nopeasti Microsoft Storen käyttämät sovellustiedostot (.appx). Voit korjata ongelman palauttamalla Kaupan oletusasetukset, tyhjentää Kaupan välimuistin ja suorittaa sitten Windows Updaten vianmäärityksen. Varmista, että Microsoft Store on suljettu, ennen kuin jatkat näillä ohjeilla.

**Vaihe 1: Palauta Microsoft Store**

**Huomautus** Tämä poistaa sovelluksen tiedot pysyvästi laitteesta, mukaan lukien mieltymyksesi ja kirjautumistietosi.

1. Valitse   >  **Aloitusasetukset-sovellussovellukset**  >    >  **& ominaisuudet.**

1. Etsi ja valitse sovellusluettelosta Microsoft Store.

1. Valitse **Lisäasetukset.**

1. Vieritä alaspäin, **valitse Palauta** ja vahvista **palautus.**

**Vaihe 2: Microsoft Storen välimuistin tyhjentäminen**

1. Avaa Suorita-valintaikkuna painamalla näppäinyhdistelmää Windows-näppäin + R.

1. Kirjoita wsreset.exe ja valitse **OK.**

1. Näyttöön avautuu tyhjä komentokehoteikkuna. Noin 10 sekunnin kuluttua ikkuna sulkeutuu ja Kauppa avautuu automaattisesti.

**Vaihe 3: Palauta Windows Update**

1. Valitse **Start**  >  **Settings**  >  **Update & Security**  >  **Troubleshoot**.

1. Vieritä alaspäin, **valitse Windows Update** luettelosta ja valitse Suorita **vianmääritys.**

1. Käynnistä tietokone uudelleen ja tarkista, onko ongelma yhä ongelmassa.

