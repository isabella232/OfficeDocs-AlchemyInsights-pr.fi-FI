---
title: Yhteyskäytännön ratkaiseminen
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746753"
---
# <a name="fix-connection-policy"></a>Yhteyskäytännön ratkaiseminen

Sähköposti on merkitty turvalliseksi ja toimitettu käyttäjän Saapuneet-kansioon, koska lähettävä IP-osoite on merkitty turvalliseksi Yhteyssuodatin-käytännön avulla. Voit tarkistaa käytännön seuraavasti:

1. Siirry [Office 365:n tietoturva- & yhteensopivuuskeskukseen](https://go.microsoft.com/fwlink/p/?linkid=2077143)ja siirry sitten **uhkien**  >  **hallintakäytäntöön**  >  [roskapostin estoon.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Valitse **Mukautettu-välilehdessä** **Yhteyssuodatin-käytäntö** ja valitse sitten **Muokkaa käytäntöä.**
3. Tarkista **SALLITTUJEN IP-osoitteiden** luettelo. Katso, **onko turvallinen luettelo** käytössä.

    > [!NOTE]
    > Microsoft tilaa luotettavien lähettäjien kolmannen osapuolen lähteitä. Jos **turvallinen luettelo** on käytössä, näitä luotettavia lähettäjiä ei merkitä vahingossa roskapostiksi. Suosittelemme tämän asetuksen valitsemista, koska se vähentää vastaanottamiasi virheellisiä positiivisia viestejä (roskapostiksi luokiteltuja hyviä viestejä).
