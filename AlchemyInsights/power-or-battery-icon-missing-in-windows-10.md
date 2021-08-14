---
title: Virta- tai akkukuvake puuttuu Windows 10:ssä
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
- "9002953"
- "5655"
ms.openlocfilehash: 82d41844de1eafdf7e0cc38f91416f3b71868e3d5d1b3eb8be0f10abd701ddc8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973318"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a>Virta- tai akkukuvake puuttuu Windows 10:ssä

Jos Windows 10 -laitteessasi (kuten kannettavassa tietokoneessa, tabletissa tai UPS:ään USB:n avulla yhdistetyssä PC-tietokoneessa) on akku, tehtäväpalkissa lähellä kelloa näytetään tavallisesti virta- tai akkukuvake. Esimerkki:

![Akkukuvake](media/battery-icon.png)

Jos et näe tätä kuvaketta, se on voitu piilottaa:

1. Siirry kohtaan **[Asetukset > Mukauttaminen > Tehtäväpalkki](ms-settings:taskbar?activationSource=GetHelp)**.

2. Valitse ilmoitusalueella **Valitse, mitkä kuvakkeet näkyvät tehtäväpalkissa**.

3. Etsi luettelosta **Virta** ja muuta sen valinnaksi **Käytössä**.

    ![Virtakuvakkeen näyttäminen tehtäväpalkissa](media/power-icon-on.png)

**Vianmääritys**

Jos noudatit yllä olevia ohjeita eikä **Virta**-vaihtopainiketta näy tai se näkyy harmaana, kirjoita tehtäväpalkin hakuruutuun **laitehallinta** ja valitse sitten tulosluettelosta **Laitehallinta**. Napsauta **Akut**-kohdassa laitteesi akkua hiiren kakkospainikkeella. Valitse sitten **Poista käytöstä** ja **Kyllä**. Odota muutama sekunti, napsauta akkua hiiren kakkospainikkeella ja valitse **Ota käyttöön**. Käynnistä laite sitten uudelleen.

Jos noudatit yllä olevia ohjeita eikä akkukuvaketta näy tehtäväpalkissa, kirjoita tehtäväpalkin hakuruutuun **tehtävien hallinta** ja valitse sitten tulosluettelosta **Tehtävien hallinta**. Napsauta **Prosessit**-välilehden **Nimi**-kohdassa **Resurssienhallinta**-kohtaa hiiren kakkospainikkeella ja valitse sitten **Käynnistä uudelleen**.
