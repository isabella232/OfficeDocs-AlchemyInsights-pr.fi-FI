---
title: Dataprotectionin-BitLocker
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
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731236"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>BitLocker-Sala uksen ottaminen käyttöön Intunella

 Intune-pääte pisteen suojaus käytäntöä voidaan käyttää Windows-laitteiden BitLocker-salaus asetusten määrittämiseen. Lisä tietoja on kohdassa [Windows 10: n (tai uudemman) asetukset laitteiden suojaamiseksi Intune-toiminnolla](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Huomaa, että monet Windows 10: tä käyttävät uudet laitteet tukevat automaattista BitLocker-salausta, joka käynnistyy ilman MDM-käytäntöä. Tämä voi vaikuttaa käytäntöjen soveltamiseen, jos muut kuin oletus asetukset on määritetty. Lisä tietoja on seuraavissa usein kysytyissä kysymyksissä.
 
Lisä tietoja BitLocker-ongelmien vian määrityksestä on kohdassa [BitLocker-käytäntöjen vian määritys Microsoft Intunella](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Usein kysytyt kysymykset**

 K: mitkä Windows-versiot tukevat laitteen salausta pääte pisteen suojaus käytäntöä käyttäen?<br>
 A: asetukset Intune-pääte pisteen suojaus käytännössä on toteutettu [BitLocker-salaus menetelmän](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)avulla. Kaikki Windowsin versiot eivät tue BitLocker-salaus menetelmän tarjoajaa. <br><br>
      Tällä hetkellä seuraavat Windows-versiot ovat tuettuja: Enterprise, Education, Mobile, Mobile Enterprise ja Professional (koonti versio 1809 ja uudemmat versiot).
 
K: Jos laite on jo salattu BitLocker-Sala uksella käyttämällä käyttö järjestelmän oletus asetuksia salaus menetelmässä ja Sala kirjoituksen voimakkuus (XTS-AES-128), se soveltaa käytäntöä, jossa on käytössä eri asetukset, jolloin uudet asetukset käyttävät aseman uudelleensalausta automaattisesti.<br>
V: Ei. Jos haluat käyttää uusia cipher-asetuksia, aseman salaus on ensin purettava.<br><br>
**Huomautus:** Jos laitteessa on rekisteröity Autopilot, OOBE-toiminnon aikana suoritettava automaattinen salaus ei käynnisty, ennen kuin Intune-käytäntöä arvioidaan, jolloin käytäntöpohjaisia asetuksia voidaan käyttää käyttö järjestelmän oletus arvojen sijasta.
 
K: Jos laite salataan Intune-käytännöstä johtuvan sovelluksen avulla, salaus puretaan, kun tämä menettely tapa poistetaan?<br>
A: salaukseen liittyvän käytäntöjen poistaminen ei johda määritettyjen asemien Sala uksen purkamiseen.
 
K: Miksi Intune-yhteensopivuus käytännöt osoittavat, että laitteessani ei ole BitLocker-suojausta käytössä, vaikka se on?<br>
A: "BitLocker Enabled"-asetus Intune-yhteensopivuus käytännössä käyttää Windows Device Health-ohjelmisto (DHA)-asiakas ohjelmaa. Tämä asiakas mittaa vain laitteen tilan käynnistyksen aikana. Jos laitetta ei ole käynnistetty uudelleen, koska BitLocker-salaus on valmis, DHA-asiakas palvelu ei ilmoita BitLocker-salausta aktiivi seksi.
 
 