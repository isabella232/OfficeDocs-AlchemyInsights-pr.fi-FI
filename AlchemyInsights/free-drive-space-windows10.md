---
title: Levytilan vapauttaminen Windows 10:ssä
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
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505353"
---
# <a name="free-up-drive-space-in-windows-10"></a>Levytilan vapauttaminen Windows 10:ssä

Tässä on kaksi vaihtoehtoa levytilan vapauttamiseen Windowsissa:

- Levytilan vapauttaminen Windows 10:ssä.
- Levytilan vapauttaminen Windows 10 -päivityksille ulkoisella tallennuslaitteella.

Jos sinulla on yhä vähän levytilaa levyn uudelleenjärjestämisen jälkeen, Temp-kansiosi saattaa mahdollisesti täyttyä nopeasti Microsoft Storen käyttämillä sovellustiedostoilla (.appx). Voit korjata ongelman palauttamalla Storen, tyhjentämällä Storen välimuistin ja suorittamalla sitten Windows Updaten vianmäärityksen. Varmista, että Microsoft Store on suljettu, ennen kuin käytät näitä vaiheita.

**Vaihe 1: Palauta Microsoft Store**

**Huomautus** Tämä poistaa pysyvästi sovellustiedot laitteesta, mukaan lukien asetukset ja kirjautumistiedot.

1. Valitse **Aloitus** > **Asetukset** > **Sovellukset** > **Sovellukset ja ominaisuudet**.

1. Etsi ja valitse sovellusluettelosta Microsoft Store.

1. Valitse **Lisäasetukset**.

1. Vieritä alaspäin ja valitse **Palauta**, ja valitse sitten **Vahvista palautus**.

**Vaihe 2: Microsoft Storen välimuistin tyhjentäminen**

1. Avaa Suorita-valintaikkuna painamalla näppäinyhdistelmää Windows-näppäin + R.

1. Kirjoita wsreset.exe ja valitse **OK**.

1. Tyhjä komentokehoteikkuna avautuu. Noin 10 sekunnin kuluttua ikkuna sulkeutuu, ja Store avautuu automaattisesti.

**Vaihe 3: Palauta Windows Update**

1. Valitse **Aloitus** > **Asetukset** > **Päivittäminen ja suojaus** > **Vianmääritys**.

1. Vieritä alaspäin ja valitse luettelosta **Windows Update**, ja valitse **Suorita vianmääritys**.

1. Käynnistä tietokone uudelleen ja tarkista, ilmeneekö ongelma edelleen.

