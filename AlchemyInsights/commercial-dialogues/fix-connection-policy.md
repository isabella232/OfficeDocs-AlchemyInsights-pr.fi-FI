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
ms.openlocfilehash: d27d570a7bc0f2c1081ba7fd52264a20bf25a453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314841"
---
# <a name="fix-connection-policy"></a>Yhteyskäytännön korjaus

Sähköpostiviesti merkittiin turvallisiksi ja toimitettiin käyttäjän Saapuneet-kansioon, koska lähde-IP-osoite oli merkitty turvalliseksi oletusarvoisen yhteyssuodatinkäytännön mukaisesti. Voit tarkistaa käytännön seuraavasti:

1. Siirry Microsoft 365 Defender -portaalissa kohtaan <https://security.microsoft.com/> **Sähköposti- &-&** \> **Käytännöt-kohdassa** Sääntöjen uhkien käytännöt roskapostin \>  \>  esto. 

   Jos haluat siirtyä suoraan **Roskapostin käytännöt -sivulle,** käytä <https://security.microsoft.com/antispam> -

2. Valitse **Roskapostin estokäytännöt** -sivulla käytäntö nimeltä **Yhteyssuodatinkäytäntö (oletus)** napsauttamalla käytännön nimeä.

3. Valitse näyttöön tulevassa tietojen pikaikkunassa **Yhteyden suodatus** -osassa Muokkaa **yhteyssuodatinkäytäntöä.**

4. Tarkista Salli viestit  aina seuraavista IP-osoitteista tai osoitealueista -kohdan merkinnät ja tarkista, **onko Ota käyttöön turvallinen** luettelo -vaihtoehto valittuna.

   **Huomautus:** Microsoft tilaa luotettavien lähettäjien kolmannen osapuolen lähteitä. Jos turvallinen luettelo on käytössä, näitä luotettavia lähettäjiä ei merkitä vahingossa roskapostiksi. Suosittelemme tämän asetuksen valitsemista, koska se vähentää vastaanottattamiasi virheellisiä positiivisia viestejä (hyviä viestejä, jotka luokitellaan roskapostiksi).

Lisätietoja on kohdassa [Yhteyden suodatuksen määrittäminen.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy)
