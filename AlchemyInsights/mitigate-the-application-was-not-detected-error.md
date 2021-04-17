---
title: Ehkäise Sovellusta ei tunnistettu -virhe
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
- "9000171"
- "1712"
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836348"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Ehkäise “Sovellusta ei tunnistettu” -virhe

Sovelluksen asennusvirhe: “Sovellusta ei tunnistettu, kun asennus on suoritettu onnistuneesti” Intunen raportoimana. Se saattaa näkyä kaikissa tärkeimmissä OS-ympäristöissä (Windows, iOS ja Android).

Tämän virheen aiheuttavat yleisimmät skenaariot ovat seuraavat:

- Sovellus on päivitetty Intunen ulkopuolella (kolmannen osapuolen sovelluskaupasta) ensimmäisen käyttöönoton jälkeen. Esimerkiksi jotkin sovellukset, kuten Google Chrome, voivat tehdä automaattisia päivityksiä.
- Käyttäjä on poistanut sovelluksen asennuksen ensimmäisen asennuksen jälkeen.

Jos haluat estää ongelman, tee ensin arvio siitä, mitä laitteita on tarkasteltava, jotta voit määrittää, missä skenaariossa virhe ilmenee.

- Jos sovellus on päivitetty Intunen ulkopuolella, sovelluksen käyttöönoton voi määrittää ohittamaan sovellusversion. Se tapahtuu määrittämällä kohdassa **Sovelluksen määritys > Sovelluksen tiedot** **Hylkää sovellus** valinta **Kyllä**.
- Asiakasta kohdennettaessa saattaa olla tarpeen ottaa sovellus käyttöön pakolliseksi ja varmistaa, että uusin versio on otettu käyttöön.
- Vaihtoehtoisesti voit käyttää iOS-ympäristössä **Automaattinen päivitys** -toimintoa, joka on liitetty Applen volyymiosto-ohjelmaan, joka voidaan määrittää päivittämään automaattisesti uusiin sovellusversioihin, kun ne ovat saatavilla.

Jos haluat lisätietoja sovellusten asennusongelmien vianmäärityksestä, lue [Sovellusten asennusongelmien vianmääritys](https://docs.microsoft.com/intune/troubleshoot-app-install).
