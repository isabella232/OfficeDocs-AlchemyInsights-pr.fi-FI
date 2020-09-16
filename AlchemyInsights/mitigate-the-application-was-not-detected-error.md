---
title: Ehkäise Sovellusta ei tunnistettu -virhe
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
- "9000171"
- "1712"
ms.openlocfilehash: 498c2ec78bc9f4a7bc7d77d12b488be2cf0bf79a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666975"
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
