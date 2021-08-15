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
ms.openlocfilehash: 34b2024257c88512db170cbb0e672c1628ad8e3935342f87c5032492e1ad0259
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026111"
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
