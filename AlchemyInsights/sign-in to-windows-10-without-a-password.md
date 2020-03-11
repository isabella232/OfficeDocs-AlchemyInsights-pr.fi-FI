---
title: Kirjautuminen Windows 10:een ilman salasanaa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588278"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Kirjautuminen Windows 10:een ilman salasanaa

Jotta sinun ei tarvitsisi kirjoittaa salasanaa Windowsin käynnistyksen yhteydessä, suosittelemme, että käytät jotakin Windows Hello -suojatun kirjautumisvaihtoehdon, kuten PIN-koodin, kasvojentunnistuksen tai sormenjäljen, jos se on käytettävissä. Jos haluat todella poistaa suojatun kirjautumisen käytöstä, katso alla olevat "Kirjaudu automaattisesti Windows 10:een" -ohjeet.

**Suojaa Windows Hello vaihtoehtoja tilin salasana**

Siirry **kohtaan Asetukset > Tilit > kirjautumisasetukset** (tai klikkaa [tästä](ms-settings:signinoptions?activationSource=GetHelp)). Käytettävissä olevat kirjautumisvaihtoehdot näkyvät luettelossa. Esimerkki:

![Kirjautumisasetukset.](media/sign-in-options.png)

Määritä se napsauttamalla tai napauttamalla jotakin vaihtoehtoa. Kun seuraavan kerran käynnistät Windowsin tai avaat sen lukituksen, voit käyttää uutta vaihtoehtoa salasanan sijaan. 

**Kirjautuminen automaattisesti Windows 10:een**

**Huomautus:** Automaattinen sisäänkirjautuminen on kätevää, mutta siinä on tietoturvariski, varsinkin jos useat henkilöt ovat käytettävissä tietokoneessasi. 

1. Napsauta tai napauta **tehtäväpalkin** Käynnistä-painiketta.

2. Kirjake **netplwiz** ja humauttaa Astua avain jotta auki Käyttäjä Selittää asian akkuna.

3. Valitse **Käyttäjätilit**-kohdassa tili, johon haluat kirjautua automaattisesti, kun Windows käynnistyy.

4. Poista "Käyttäjien on annettava käyttäjänimi ja salasana käyttää tätä tietokonetta" -valintaruudun valinta.

    ![Käyttäjien on annettava käyttäjänimi ja salasana -vaihtoehto.](media/users-must-enter-username.png)

5. Valitse **OK**. Sinua pyydetään antamaan ja vahvistamaan valitsemasi tilin salasana. Lopeta valitsemalla **OK.** Kun Windows 10 käynnistyy seuraavan kerran, se kirjautuu automaattisesti valitsemaasi tiliin.
