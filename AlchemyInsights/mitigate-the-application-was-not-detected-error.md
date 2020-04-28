---
title: Ehkäise Sovellusta ei tunnistettu -virhe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810481"
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
