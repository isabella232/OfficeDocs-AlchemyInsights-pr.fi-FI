---
title: Sormenjälkilukituksen poistaminen -asetuksen käyttäminen Windows 10:ssä
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588313"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Sormenjälkilukituksen poistaminen -asetuksen käyttäminen Windows 10:ssä

**Windows Hello Fingerprintin ottaminen käyttöön**

Jos haluat poistaa Windows 10:n lukituksen sormenjäljen avulla, sinun on määritettävä Windows Hello Fingerprint lisäämällä (antamalla Windowsin oppia tunnistamaan) vähintään yksi sormi. 

1. Siirry **kohtaan Asetukset > Tilit > kirjautumisasetukset** (tai klikkaa [tästä](ms-settings:signinoptions?activationSource=GetHelp)). Käytettävissä olevat kirjautumisvaihtoehdot näkyvät luettelossa. Esimerkki:

    ![Kirjautumisasetukset.](media/sign-in-options.png)

2. Valitse **Windows Hello Fingerprint**ja valitse sitten **Määritä**. Valitse Windows Hello -asennusikkunassa **Aloita**. Sormenjälkitunnistin aktivoituu, ja sinua pyydetään sijoittamaan sormesi anturiin:

   ![Sormenjälkitunnistin.](media/fingerprint-sensor.png)

3. Noudata ohjeita, jotka pyytävät sinua toistuvasti skannata sormesi. Kun tämä on valmis, voit lisätä muita sormia, joita haluat ehkä käyttää kirjautumiseen. Kun seuraavan kerran kirjaudut Windows 10:een, voit käyttää sitä käyttämällä sormenjälkeäsi.

**Windows Hello Fingerprint ei ole käytettävissä kirjautumisvaihtoehtona**

Jos Windows Hello Fingerprint -toimintoa ei näytetä **vaihtoehtona kirjautumisasetuksissa**, Windows ei ole tietoinen tietokoneeseen liitetystä sormenjälkilukijasta/skannerista tai että järjestelmäkäytäntö estää sen käytön (jos esimerkiksi tietokoneesi on työpaikan hallinnassa). Vianmääritys: 

1. Valitse **tehtäväpalkin Aloitus-painike** ja etsi **Laitehallinta**.

2. Avaa **Laitehallinta**napsauttamalla tai napauttamalla .

3. Laajenna Laitehallinnassa Biometriset laitteet napsauttamalla sen nuolenta.

   ![Biometriset laitteet.](media/biometric-devices.png)

4. Sormenjälkiskannerin pitäisi olla biometrinen laite, kuten Synaptics WBDI -skanneri:

   ![Biometriset laitteet.](media/biometric-devices-expanded.png)

5. Jos sormenjälkiskanneria ei näytetä ja skanneri on integroitu tietokoneeseen, siirry tietokoneen valmistajan verkkosivustoon. Etsi asennettavaksi asennettavaskanneri tietokoneen mallista Windows 10 -ohjainta.

6. Jos skanneri on erillään tietokoneesta (liitetty USB:n kautta), siirry skannerin valmistajan verkkosivustoon ja etsi ja asenna Windows 10 -laiteohjainohjelmisto skannerimallillesi.
