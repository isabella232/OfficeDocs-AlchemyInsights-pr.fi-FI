---
title: SharePoint Onlinen termi säilöstä puuttuvat ehdot
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750448"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>BitLocker-Sala uksen ottaminen käyttöön Intunella

Intune-pääte pisteen suoja uksen avulla voit määrittää Boitlocker-salaus asetukset Windows-laitteille kohdassa: Windows10 (ja uudemmat) asetukset, jotka suojaavat laitteita Intunea käyttäen

Huomaa, että monet Windows 10: tä käyttävät uudet laitteet tukevat automaattista BitLocker-salausta, joka käynnistyy ilman MDM-käytäntöä. Tämä voi vaikuttaa käytäntöjen soveltamiseen, jos muut kuin oletus asetukset on määritetty. Katso lisä tietoja usein kysytyistä kysymyksistä.


Usein kysytyt kysymykset   k: mitkä Windows-versiot tukevat laitteen salausta pääte pisteen suojaus käytäntöä käyttäen?
 A: asetukset Intune-pääte pisteen suojaus käytännössä on toteutettu BitLocker-salaus menetelmän avulla.Kaikki versiot eivät tue BitLocker-salaus menetelmän tarjoajaa. 
      Tällä hetkellä Windows-versiot: Enterprise; Koulutus, matka Puhelin, mobiilisovellus ja Professional (koonti versio 1809 alkaen) ovat tuettuja.




K: Jos laite on jo salattu BitLocker-Sala uksella käyttämällä käyttö järjestelmän oletus asetuksia salaus menetelmässä ja Sala kirjoituksen voimakkuus (XTS-AES-128), käytetään käytäntöä, jossa on eri asetukset, jotka automaattisesti käyttävät aseman uudelleensalausta uusilla asetuksilla?

V: Ei. Uuden salaus asetuksen käyttäminen edellyttää, että aseman salaus on ensin purettava.

Huomautus OOBE-toiminnon aikana käyttöön otetuista laitteista ei käynnistetä automaattista salausta, ennen kuin Intune-käytäntöä arvioidaan, jolloin käytäntöpohjaisia asetuksia voidaan käyttää käyttö järjestelmän oletus asetusten sijasta.




K jos laite salataan Intune-käytäntöjen soveltamisen seura uksena, salaus puretaan, kun tämä menettely tapa poistetaan?

A: Sala ukseen liittyvän käytäntöjen poistaminen ei johda määritettyjen asemien Sala uksen purkamiseen.




K: Miksi Intune-yhteensopivuus käytännöt osoittavat, että laitteessani ei ole "BitLocker käytössä", mutta se on?

A: "BitLocker Enabled"-asetus Intune-yhteensopivuus käytännössä hyödyntää Windows Device Health-tieto asema (DHA)-asiakas ohjelmaa. Tämä asiakas mittaa vain laitteen tilan käynnistyksen aikana. Jos laitetta ei ole käynnistetty uudelleen, koska BitLocker-salaus on valmis, DHA-asiakas palvelu ei ilmoita BitLocker-salausta aktiivi seksi.