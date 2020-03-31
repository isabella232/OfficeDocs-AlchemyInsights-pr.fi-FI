---
title: Kaatuuko Teams?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030586"
---
# <a name="teams-client-crashing"></a>Kaatuuko Teams?

Jos Teams-ohjelmasi kaatuu, kokeile seuraavia keinoja:

- Jos käytät Teams-työpöytäsovellusta, varmista, että [sovellus on täysin ajan tasalla](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Varmista, että kaikki [Office 365:n URL-osoitteet ja osoitealueet](https://docs.microsoft.com/microsoftteams/connectivity-issues) ovat käytettävissä.

- Kirjaudu sisään järjestelmänvalvojatililläsi ja tarkista [palvelun kunnon koontinäytöstä](https://docs.microsoft.com/office365/enterprise/view-service-health), että palvelussa ei ole käyttökatkoja tai rajoituksia.

 - Viimeisenä keinona voit yrittää tyhjentää Teams-ohjelman välimuistin:

    1.  Sulje Microsoft Teams -työpöytäohjelma kokonaan. Napsauta **Teamsia** hiiren kakkospainikkeella kuvakkeissa ja napsauta sitten **Lopeta**. Voit myös lopettaa prosessin täysin tehtävienhallinnassa.

    2.  Avaa Resurssienhallinta ja kirjoita %appdata%\Microsoft\teams.

    3.  Näet tässä hakemistossa seuraavia kansioita:

         - Siirry **Application Cache** -kansiossa Cache-alikansioon ja poista kaikki tiedostot tästä välimuistikansiosta:  %appdata%\Microsoft\teams\application cache\cache.

        - Poista kaikki **Blob_storage**-kansion tiedostot: %appdata%\Microsoft\teams\blob_storage.

        - Poista kaikki **Cache**-kansion tiedostot: %appdata%\Microsoft\teams\Cache.

        - Poista kaikki **databases**-kansion tiedostot: %appdata%\Microsoft\teams\databases.

        - Poista kaikki **GPUCache**-kansion tiedostot: %appdata%\Microsoft\teams\GPUCache.

        - Poista kaikki **IndexedDB**-kansion tiedostot: %appdata%\Microsoft\teams\IndexedDB.

        - Poista kaikki **Local Storage** -kansion tiedostot: %appdata%\Microsoft\teams\Local Storage.

        - Poista vielä myös kaikki **tmp**-kansion tiedostot: %appdata%\Microsoft\teams\tmp.

    4. Käynnistä Teams-ohjelma uudelleen.
