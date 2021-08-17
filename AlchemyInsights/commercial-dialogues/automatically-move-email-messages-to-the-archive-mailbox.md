---
title: Sähköpostiviestien siirtäminen arkistopostilaatikkoon automaattisesti
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 57dbfd116bbae227f2288ce23edeaaa833fadf54ca3b10b95c49512758542e32
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059223"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Sähköpostiviestien siirtäminen arkistopostilaatikkoon automaattisesti

Näin voit määrittää käytännön, joka siirtää käyttäjän vanhat sähköpostit automaattisesti arkistopostilaatikkoon:

1. Siirry [**tietoturvatietojen & tietojen hallinta**](https://go.microsoft.com/fwlink/p/?linkid=2077143)-arkistoon ja tarkista, että käyttäjälle on otettu käyttöön  >    >   arkistopostilaatikko. Jos näin ei ole, valitse **varoitusruudussa** Ota käyttöön **ja** sitten Kyllä.
2. Siirry [**Exchange hallintakeskukseen > säilytystunnisteiden yhteensopivuuden > hallintakeskuksessa.**](https://go.microsoft.com/fwlink/?linkid=2059104)
3. Valitse + -kuvake ja käytä **automaattisesti koko postilaatikkoa.**
4. Anna säilytystunnisteeseen nimi ja valitse **Siirrä arkistoon**. Määritä säilytysjaksolle aika, kuten 90 päivää. Valitse **Tallenna**.
5. Luo nyt säilytyskäytäntö: valitse **säilytyskäytännöt** ja lisää uusi käytäntö valitsemalla kuvake.
6. Määritä säilytyskäytäntöön nimi, etsi juuri luomasi säilytystunniste napsauttamalla ja vierittämällä. Valitse **Tallenna**.
7. Ota lopuksi säilytyskäytäntö käyttöön käyttäjän postilaatikossa: siirry edelleen Exchange hallintakeskuksessa **vastaanottajien**  >  **postilaatikoihin**. Valitse kaikki käyttäjät, joissa haluat käyttää käytäntöä, ja valitse sitten **Muokkaa** (kynäkuvake).
8. Valitse valintaikkunassa **Postilaatikon ominaisuudet**. Ota **Säilytyskäytäntö-kohdassa** käyttöön juuri luomasi > **Tallenna**.
9. Ohjeet käytännön käyttöön kaikille käyttäjille ovat kohdassa [Säilytyskäytännön käyttäminen postilaatikoissa.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
