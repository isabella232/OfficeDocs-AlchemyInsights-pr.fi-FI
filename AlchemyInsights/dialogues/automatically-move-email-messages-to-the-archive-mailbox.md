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
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50525098"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Sähköpostiviestien siirtäminen arkistopostilaatikkoon automaattisesti

Näin voit määrittää käytännön, joka siirtää käyttäjän vanhat sähköpostiviestit automaattisesti arkistopostilaatikkoon:

1. Siirry [**tietoturvatietojen & tietojen**](https://go.microsoft.com/fwlink/p/?linkid=2077143)hallinta-arkistoon ja tarkista, että käyttäjälle  >    >   on otettu käyttöön arkistopostilaatikko. Jos näin ei ole,  valitse **varoitusruudussa** Ota käyttöön ja sitten Kyllä.
2. Siirry [**Exchange-hallintakeskukseen > ja säilytystunnisteiden > hallintakeskuksessa.**](https://go.microsoft.com/fwlink/?linkid=2059104)
3. Valitse + -kuvake ja valitse sitten **automaattisesti koskee koko postilaatikkoa.**
4. Anna säilytystunnisteeseen nimi ja valitse **Siirrä arkistoon.** Anna säilytysjaksolle aika, jonka haluat, kuten 90 päivää. Valitse **Tallenna**.
5. Luo nyt säilytyskäytäntö: valitse **säilytyskäytännöt** ja lisää uusi käytäntö valitsemalla kuvake.
6. Määritä säilytyskäytäntöön nimi, etsi ja lisää juuri luomasi säilytystunniste napsauttamalla ja vierittämällä. Valitse **Tallenna**.
7. Ota lopuksi säilytyskäytäntö käyttöön käyttäjän postilaatikossa: siirry edelleen Exchange-hallintakeskuksessa vastaanottajien   >  **postilaatikoihin.** Valitse kaikki käyttäjät, joissa haluat käyttää käytäntöä, ja valitse sitten **Muokkaa** (kynäkuvake).
8. Valitse valintaikkunassa **postilaatikon ominaisuudet.** Ota **Säilytyskäytäntö-kohdassa** käyttöön juuri luomasi > **tallentaminen.**
9. Ohjeet käytännön käyttöönottamisen käyttöön kaikille käyttäjille ovat ohjeaiheessa [Säilytyskäytännön käyttäminen postilaatikoissa.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
