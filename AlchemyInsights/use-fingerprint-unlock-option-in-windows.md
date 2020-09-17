---
title: 'Sormen jälkien lukituksen poistaminen Windows 10: ssä'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795241"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Sormen jälkien lukituksen poistaminen Windows 10: ssä

**Windows Hello-sormen jäljen ottaminen käyttöön**

Jos haluat poistaa Windows 10: n lukituksen sormen jäljen avulla, sinun on määritettävä Windows Hello-sormen jälki lisäämällä (antaen Windowsin oppia tunnistamaan) vähintään yhdellä sormella. 

1. Siirry kohtaan **asetukset > asiakkaat > kirjautumisvaihtoehdot** (tai napsauta [tätä](ms-settings:signinoptions?activationSource=GetHelp)). Käytettävissä olevat kirjautumisvaihtoehdot näkyvät luettelossa. Esimerkiksi:

    ![Kirjautumisvaihtoehdot.](media/sign-in-options.png)

2. Napsauta tai napauta **Windows Hello-sormen jälki**ja valitse sitten **Määritä**. Valitse Windows Hello Setup- **ikkunassa aloittaminen.** Sormen jälki tunnistin aktivoituu, ja sinua pyydetään antamaan sormi tunnistimeen:

   ![Sormen jälki tunnistin.](media/fingerprint-sensor.png)

3. Noudata ohjeita, jotka pyytävät sinua skannaamaan sormella toistuvasti. Kun tämä on valmis, voit halutessasi lisätä muita sormia, joita haluat käyttää kirjautumiseen. Kun seuraavan kerran kirja udut sisään Windows 10: een, voit käyttää sormen jälkeä.

**Windows Hello-sormen jälki ei ole käytettävissä kirjautumisvaihtoehtona**

Jos Windows Hello-sormen jälki ei näy vaihto ehtona **kirjautumisasetuksissa**, Windows ei ole tietoinen tieto koneeseesi liitetystä sormenjälkilukijasta tai skannerista tai järjestelmä käytäntö estää sen käytön (Jos esimerkiksi työpaikkasi hallitsee tieto konettasi). Vian määritys: 

1. Valitse tehtävä palkin **Käynnistä** -painike ja Etsi **laite hallintaa**.

2. Avaa **laite hallintaa**napsauttamalla tai napauttamalla.

3. Laajenna laite hallinnasta biometriset laitteet napsauttamalla sen Chevron-merkkiä.

   ![Biometriset laitteet.](media/biometric-devices.png)

4. Sormenjälkiskannerin pitäisi näkyä biometrisenä laitteena, kuten Synaptics WFDI Scanner:

   ![Biometriset laitteet.](media/biometric-devices-expanded.png)

5. Jos sormenjälkiskannerisi ei näy ja skanneri on integroitu tieto koneeseesi, siirry tieto koneen valmistajan sivustoon. Etsi tieto koneen mallin teknisen tuen osasta Windows 10-ohjain asennettavia skannereita varten.

6. Jos skanneri on erillään tieto koneesta (liitetty USB-liitännän kautta), Etsi ja asenna Windows 10: n laite ohjain ohjelmisto skannerin mallia varten laitteen valmistajan sivustosta.
