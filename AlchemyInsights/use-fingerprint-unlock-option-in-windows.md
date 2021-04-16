---
title: Sormenjälkilukituksen käyttö Windows 10:ssä
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
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796674"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Sormenjälkilukituksen käyttö Windows 10:ssä

**Windows Hellon sormenjäljen ottaminen käyttöön**

Jotta voit poistaa Windows 10:n lukituksen sormenjäljen avulla, sinun on määritettävä Windows Hello Fingerprint lisäämällä (antamalla Windowsin opetella tunnistamaan) vähintään yksi sormi. 

1. Siirry asetukset **> tilit > kirjautumisasetukset** (tai napsauta [tätä).](ms-settings:signinoptions?activationSource=GetHelp) Käytettävissä olevat kirjautumisvaihtoehdot tulevat luetteloon. Esimerkiksi:

    ![Kirjautumisasetukset.](media/sign-in-options.png)

2. Napsauta tai napauta **Windows Hellon sormenjälkeä** ja **valitse sitten Määritä**. Valitse Windows Hellon määritysikkunassa **Aloita käyttö.** Sormenjälkitunnistin aktivoituu, ja sinua pyydetään asetamaan sormesi tunnistimeen:

   ![Sormenjälkitunnistin.](media/fingerprint-sensor.png)

3. Noudata ohjeita, jotka pyytävät sinua skannaamaan sormella toistuvasti. Kun tämä on valmis, voit lisätä muita sormia, joita haluat ehkä käyttää kirjautumiseen. Kun seuraavan kerran kirjaudut Windows 10:ssä, voit käyttää sormenjälkeäsi.

**Windows Hellon sormenjälki ei ole käytettävissä kirjautumisvaihtoehtona**

Jos Windows Hello Fingerprint ei näy kirjautumisasetusten vaihtoehtona, Windows ei ole tietoinen tietokoneeseen liitetystä sormenjälkilukijasta tai että järjestelmäkäytäntö estää sen käytön (jos esimerkiksi työpaikkasi hallinnoi tietokonetta). Vianmääritys: 

1. Valitse **tehtäväpalkin** Käynnistä-painike ja etsi **Laitehallinta.**

2. Avaa Laitehallinta **napsauttamalla tai napauttamalla**.

3. Laajenna Laitehallinnassa Biometriset laitteet napsauttamalla sen chevron-kohtaa.

   ![Biometriset laitteet.](media/biometric-devices.png)

4. Sormenjälkiskannerilla pitäisi olla biometrinen laite, kuten Synaptics WBDI -skanneri:

   ![Biometriset laitteet.](media/biometric-devices-expanded.png)

5. Jos sormenjälkilukija ei ole näkyvissä ja skanneri on integroitu tietokoneeseen, siirry tietokoneen valmistajan sivustoon. Etsi PC-mallin teknisestä tuesta Windows 10 -ohjainta, jonka voit asentaa.

6. Jos skanneri on erillinen tietokoneesta (USB:n kautta liitettynä), etsi ja asenna Windows 10 :n laiteohjainohjelmisto skannerimallia varten skannerivalmistajan sivustosta.
