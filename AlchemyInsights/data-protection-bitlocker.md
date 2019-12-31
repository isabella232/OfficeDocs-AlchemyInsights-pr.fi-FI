---
title: Tieto suoja-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908707"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>BitLocker-Sala uksen ottaminen käyttöön Intune-avulla

 Intune-pääte pisteiden suojaus käytäntöä voidaan käyttää Windows-laitteiden BitLocker-salaus asetusten määrittämiseen. Lisä tietoja on Ohje aiheessa [Windows 10 (ja uudemmat)-asetukset suojaamaan laitteita Intune-toiminnolla](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Huomaa, että monet uudemmat Windows 10-laitteet tukevat automaattista BitLocker-salausta, joka käynnistyy ilman MDM-käytännön soveltamista. Tämä saattaa vaikuttaa käytännön soveltamiseen, jos muita kuin oletus asetuksia on määritetty. Katso lisä tietoja seuraavista usein kysytyistä kysymyksistä.
 
Lisä tietoja BitLocker-ongelmien vian määrityksestä on kohdassa [Microsoft Intune-työkalun BitLocker-käytäntöjen vian määritys](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Usein kysytyt kysymykset**

 K: mitkä Windows-versiot tukevat laitteen salausta pääte pisteiden suojaus käytännön avulla?<br>
 V: Intune-pääte pisteen suojaus käytännön asetukset toteutetaan [BitLocker-salaus](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)menetelmän avulla. Kaikki Windowsin versiot ja koonti versiot eivät tue BitLocker-SALAUS menetelmän versiota. <br><br>
      Tällä hetkellä tuetaan seuraavia Windows-versioita: Enterprise, Education, Mobile, Mobile Enterprise ja Professional (Build 1809 ja uudemmat).
 
K: Jos laite on jo salattu BitLockerin kanssa käyttämällä käyttö järjestelmän oletus asetuksia salaus menetelmälle ja Sala kirjoituksen voimakkuudesta (XTS-AES-128), Soveltakaamme käytäntöä, jossa eri asetukset laukaisevat automaattisesti aseman uudelleen Sala uksen uusilla asetuksilla?<br>
A: ei. Jotta uusi salaus asetus voidaan ottaa käyttöön, asema on ensin purettava.<br><br>
**Huom:** Jos laite on rekisteröity automaatti ohjaukseen, OOBE-toiminnon aikana tapahtuvaa automaattista salausta ei käynnistetä, ennen kuin Intune-käytäntöä arvioidaan, jolloin käytäntöpohjaisia asetuksia voidaan käyttää käyttö järjestelmän oletus arvojen sijasta.
 
K: Jos laite salataan Intune-käytännön soveltamisen seura uksena, onko se purettava, kun kyseinen käytäntö poistetaan?<br>
A: Sala ukseen liittyvän käytännön poistaminen ei johda määritettyjen asemien Sala uksen purkamiseen.
 
K: Miksi Intune-yhteensopivuus käytäntö osoittaa, että laitteeni ei ole BitLocker käytössä, vaikka se on?<br>
V: "BitLocker Enabled"-asetus Intune Compliance-käytännössä hyödyntää Windows Device Health Attestation (DHA)-asiakasta. Tämä asiakas mittaa vain laitteen tilan käynnistyksen aikana. Jos laitetta ei ole käynnistetty uudelleen, koska BitLocker-salaus on suoritettu, DHA-asiakas palvelu ei ilmoita BitLocker-Sala uksesta aktiivi seksi.
 
 