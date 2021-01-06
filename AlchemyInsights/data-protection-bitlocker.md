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
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768814"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>BitLocker-Sala uksen ottaminen käyttöön Intunella

 Intune-pääte pisteen suojaus käytäntöä voidaan käyttää Windows-laitteiden BitLocker-salaus asetusten määrittämiseen. Lisä tietoja on kohdassa [Windows 10: n (tai uudemman) asetukset laitteiden suojaamiseksi Intune-toiminnolla](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Huomaa, että monet Windows 10: tä käyttävät uudet laitteet tukevat automaattista BitLocker-salausta, joka käynnistyy ilman MDM-käytäntöä. Tämä voi vaikuttaa käytäntöjen soveltamiseen, jos muut kuin oletus asetukset on määritetty. Lisä tietoja on seuraavissa usein kysytyissä kysymyksissä.
 
Lisä tietoja BitLocker-ongelmien vian määrityksestä on kohdassa [BitLocker-käytäntöjen vian määritys Microsoft Intunella](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Usein kysytyt kysymykset**

K: mitkä Windows-versiot tukevat laitteen salausta pääte pisteen suojaus käytäntöä käyttäen?<br>
A: asetukset Intune-pääte pisteen suojaus käytännössä on toteutettu [BitLocker-salaus menetelmän](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)avulla. Kaikki Windowsin versiot eivät tue BitLocker-salaus menetelmän tarjoajaa. <br><br>

K: Miten BitLocker voidaan ottaa käyttöön laitteissa, jotka eivät edellytä loppu käyttäjän toimia?<br>
A: niin kauan kuin tarvittavat vaatimukset täyttyvät, BitLocker-salaus voidaan ottaa käyttöön Intuneen kautta. Katso lisä tietoja laitteen vaatimuksista ja esimerkki käytäntöjen asetuksista, jotta hiljainen salaus otetaan käyttöön seuraavassa asia kirjassa: [BitLocker-Sala uksen ottaminen käyttöön](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

K: Jos laite on jo salattu BitLocker-Sala uksella käyttämällä käyttö järjestelmän oletus asetuksia salaus menetelmässä ja Sala kirjoituksen voimakkuus (XTS-AES-128), se soveltaa käytäntöä, jossa on käytössä eri asetukset, jolloin uudet asetukset käyttävät aseman uudelleensalausta automaattisesti.<br>
V: Ei. Jos haluat käyttää uusia cipher-asetuksia, aseman salaus on ensin purettava.<br><br>
**Huomautus:** Jos laitteessa on rekisteröity Autopilot, OOBE-toiminnon aikana suoritettava automaattinen salaus ei käynnisty, ennen kuin Intune-käytäntöä arvioidaan, jolloin käytäntöpohjaisia asetuksia voidaan käyttää käyttö järjestelmän oletus arvojen sijasta.
 
K: Jos laite salataan Intune-käytännöstä johtuvan sovelluksen avulla, salaus puretaan, kun tämä menettely tapa poistetaan?<br>
A: salaukseen liittyvän käytäntöjen poistaminen ei johda määritettyjen asemien Sala uksen purkamiseen.
 
K: Miksi Intune-yhteensopivuus käytännöt osoittavat, että laitteessani ei ole BitLocker-suojausta käytössä, vaikka se on?<br>
A: "BitLocker Enabled"-asetus Intune-yhteensopivuus käytännössä käyttää Windows Device Health-ohjelmisto (DHA)-asiakas ohjelmaa. Tämä asiakas mittaa vain laitteen tilan käynnistyksen aikana. Jos laitetta ei ole käynnistetty uudelleen, koska BitLocker-salaus on valmis, DHA-asiakas palvelu ei ilmoita BitLocker-salausta aktiivi seksi.
 
 