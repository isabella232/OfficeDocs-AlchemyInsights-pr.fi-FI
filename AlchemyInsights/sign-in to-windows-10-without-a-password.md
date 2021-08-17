---
title: Kirjautuminen Windows 10 ilman salasanaa
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
- "9001690"
- "3766"
ms.openlocfilehash: fbf190d433eabfee5b45348d05d918222a385314a431812aa5f5926aacf11560
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54107505"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Kirjautuminen Windows 10 ilman salasanaa

Jos haluat välttää salasanan kirjoittamisen Windows käynnistyksen yhteydessä, suosittelemme, että käytät jotain Windows Hello kirjautumisvaihtoehtoa, kuten PIN-koodia, kasvojentunnistusta tai sormenjälkeä, jos sellainen on käytettävissä. Jos haluat poistaa suojatun kirjautumisen käytöstä, katso alla olevat kirjautumisohjeet Windows 10 sisään.

**Suojaa Windows Hello vaihtoehtoja tilin salasanalle**

Siirry **Asetukset > tilit > -kohdassa** (tai napsauta [tätä).](ms-settings:signinoptions?activationSource=GetHelp) Käytettävissä olevat kirjautumisvaihtoehdot tulevat luetteloon. Esimerkiksi:

![Kirjautumisasetukset.](media/sign-in-options.png)

Määritä jokin vaihtoehdoista napsauttamalla tai napauttamalla sitä. Kun seuraavan kerran käynnistät Windows lukituksen tai poistat sen lukituksen, voit käyttää uutta vaihtoehtoa salasanan sijaan. 

**Kirjautuminen Windows 10**

**Huomautus:** Automaattinen kirjautuminen on kätevää, mutta sisältää tietoturvariskin etenkin, jos tietokone on useiden käyttäjien käytettävissä. 

1. Napsauta tai napauta **tehtäväpalkin** Käynnistä-painiketta.

2. Kirjoita **netplwiz** ja avaa Käyttäjätilit-ikkuna painamalla Enter-näppäintä.

3. Napsauta **Käyttäjätilit-kohdassa** tiliä, johon haluat kirjautua automaattisesti, kun Windows käynnistyy.

4. Poista käyttäjien on annettava käyttäjänimi ja salasana tämän tietokoneen käyttöä varten -valintaruudun valinta.

    ![Käyttäjien on annettava käyttäjänimi- ja salasana-vaihtoehto.](media/users-must-enter-username.png)

5. Napsauta **OK**. Sinua pyydetään antamaan ja vahvistamaan valitsemasi tilin salasana. Lopeta **valitsemalla OK.** Kun Windows 10 seuraavan kerran, se kirjautuu automaattisesti sisään valitsemallesi tilille.
