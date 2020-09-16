---
title: 'Kirjautuminen Windows 10: een ilman Sala sanaa'
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
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719950"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Kirjautuminen Windows 10: een ilman Sala sanaa

Jos haluat välttyä kirjoittamasta Sala sanaa Windowsin käynnistyessä, suosittelemme, että käytät jotakin Windows Hello-kirjautumisvaihtoehtoa, kuten PIN-koodi, kasvojentunnistus tai sormen jälki, jos se on käytettävissä. Jos haluat todella poistaa suojatun kirjautumisen käytöstä, Lue ohjeet kohdasta "Kirjautuminen Windows 10: een automaattisesti".

**Secure Windows Hello-vaihto ehdot tilin Sala sanaksi**

Siirry kohtaan **asetukset > asiakkaat > kirjautumisvaihtoehdot** (tai napsauta [tätä](ms-settings:signinoptions?activationSource=GetHelp)). Käytettävissä olevat kirjautumisvaihtoehdot näkyvät luettelossa. Esimerkiksi:

![Kirjautumisvaihtoehdot.](media/sign-in-options.png)

Voit määrittää sen napsauttamalla tai napauttamalla jotakin vaihto ehtoa. Kun seuraavan kerran käynnistät tai avaat Windowsin, voit käyttää uutta vaihto ehtoa Sala sanan sijaan. 

**Kirjautuminen automaattisesti Windows 10: een**

**Huomautus**: Automaattinen sisäänkirjautuminen on kätevää, mutta se sisältää tieto turva riskin etenkin, jos tieto koneesi on usean henkilön käytettävissä. 

1. Napsauta tai napauta tehtävä palkin **Käynnistä** -painiketta.

2. Kirjoita **netplwiz** ja avaa käyttäjä tunnukset-ikkuna painamalla ENTER-näppäintä.

3. Valitse **käyttäjä tilit**-kohdassa tili, johon haluat kirja utua automaattisesti, kun Windows käynnistyy.

4. Poista "käyttäjien on annettava käyttäjä nimi ja sala sana, jotta voit käyttää tätä tieto konetta"-valinta neliötä.

    ![Käyttäjien on annettava käyttäjä nimi ja sala sana-vaihto ehto.](media/users-must-enter-username.png)

5. Valitse **OK**. Sinua pyydetään antamaan ja vahvistamaan valitsemasi tilin sala sana. Valitse **OK** , jos haluat viimeistellä. Kun Windows 10 käynnistetään seuraavan kerran, se kirjautuu automaattisesti valitsemaasi tiliin.
