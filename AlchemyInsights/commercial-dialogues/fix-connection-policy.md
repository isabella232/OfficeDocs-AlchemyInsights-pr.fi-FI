---
title: Yhteyskäytännön korjaus
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
- "9000760"
- "7391"
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988098"
---
# <a name="fix-connection-policy"></a>Yhteyskäytännön korjaus

Sähköpostiviesti merkittiin turvallisiksi ja toimitettiin käyttäjän Saapuneet-kansioon, koska lähettävä IP-osoite oli merkitty turvalliseksi Yhteyssuodatin-käytännön avulla. Voit tarkistaa käytännön seuraavasti:

1. Siirry Office 365 [tietoturva- & yhteensopivuuskeskukseen](https://go.microsoft.com/fwlink/p/?linkid=2077143)ja siirry sitten Threat Management Policy Anti-spam (Uhkien   >  **hallintakäytäntö**  >  [roskapostin esto) -keskukseen.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Valitse **Mukautettu-välilehdessä** **Yhteyssuodatinkäytäntö** ja valitse sitten **Muokkaa käytäntöä**.
3. Tarkista **SALLITTUJEN IP-osoitteiden** luettelo. Katso, **onko Lokero otettu** käyttöön.

    > [!NOTE]
    > Microsoft tilaa luotettavien lähettäjien kolmannen osapuolen lähteitä. Jos **Lokero** on otettu käyttöön, näitä luotettavia lähettäjiä ei merkitä vahingossa roskapostiksi. Suosittelemme tämän asetuksen valitsemista, koska se vähentää vastaanottattamiasi virheellisiä positiivisia viestejä (roskapostiksi luokiteltuja hyviä viestejä).
