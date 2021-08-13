---
title: Käytä sormenjäljen avausasetusta Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: a171d889705a0035981465bdaa5a8f07b9d2eb7200ba4c948f2aaccbf2cc0a21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971900"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Käytä sormenjäljen avausasetusta Windows 10

**Sormenjäljen Windows Hello ottaminen käyttöön**

Jotta voit Windows 10 sormenjäljen lukituksen, sinun on määritettävä Windows Hello Sormenjälki lisäämällä (Windows tunnistamaan) vähintään yksi sormi. 

1. Siirry **Asetukset > tilit > -kohdassa** (tai napsauta [tätä).](ms-settings:signinoptions?activationSource=GetHelp) Käytettävissä olevat kirjautumisvaihtoehdot tulevat luetteloon. Esimerkiksi:

    ![Kirjautumisasetukset.](media/sign-in-options.png)

2. Valitse Windows Hello **sormenjälki ja** valitse **sitten Määritä**. Valitse Windows Hello-ikkunassa **Aloita.** Sormenjälkitunnistin aktivoituu, ja sinua pyydetään asetamaan sormesi tunnistimeen:

   ![Sormenjälkitunnistin.](media/fingerprint-sensor.png)

3. Noudata ohjeita, jotka pyytävät sinua skannaamaan sormella toistuvasti. Kun tämä on valmis, voit lisätä muita sormia, joita haluat ehkä käyttää kirjautumiseen. Kun seuraavan kerran kirjaudut Windows 10, voit käyttää sormenjälkeäsi.

**Windows Hello Sormenjälki ei ole käytettävissä kirjautumisvaihtoehtona**

Jos Windows Hello Fingerprint ei näy kirjautumisasetusten vaihtoehtona, Windows ei ole tietoinen tietokoneeseen liitetystä sormenjälkilukijasta tai että järjestelmäkäytäntö estää sen käytön (jos esimerkiksi tietokonetta hallitaan työpaikallasi). Vianmääritys: 

1. Valitse **tehtäväpalkin** Käynnistä-painike ja etsi **Laitehallinta.**

2. Avaa Laitehallinta **napsauttamalla tai napauttamalla**.

3. Laajenna Laitehallinnassa Biometriset laitteet napsauttamalla sen chevron-kohtaa.

   ![Biometriset laitteet.](media/biometric-devices.png)

4. Sormenjälkiskannerilla pitäisi olla biometrinen laite, kuten Synaptics WBDI -skanneri:

   ![Biometriset laitteet.](media/biometric-devices-expanded.png)

5. Jos sormenjälkilukija ei ole näkyvissä ja skanneri on integroitu tietokoneeseen, siirry tietokoneen valmistajan sivustoon. Etsi PC-mallin teknisestä tuesta Windows 10 skanneri, jonka voit asentaa.

6. Jos skanneri on erillinen tietokoneesta (USB:n kautta liitettynä), siirry skannerin valmistajan sivustoon ja etsi ja asenna Windows 10-ohjainohjelmisto skannerimallia varten.
