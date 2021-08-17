---
title: Termit puuttuvat SharePoint termisäilöstä
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
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106423"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>BitLocker-salauksen ottaminen käyttöön Intunen avulla

Intune Endpoint Protection-käytännön avulla voidaan määrittää Boitlocker-salausasetukset Windows-laitteille seuraavassa kuvatulla tavalla: Windows10:n (ja uudemman) laitteen suojaaminen Intunen avulla

Muista, että monet uudempia laitteita, joissa Windows 10, tukevat automaattista bitlocker-salausta, joka käynnistyy ilman MDM-käytännön sovellusta. Tämä voi vaikuttaa käytännön sovellukseen, jos oletusasetuksia ei ole määritetty. Lisätietoja on usein kysytyissä kysymyksissä.


Usein kysytyt kysymykset: Mitkä Windows tukevat laitesalausta Endpoint Protection käytäntöä?
V: Intune-Endpoint Protection asetukset on otettu käyttöön Bitlocker-CSP:n avulla.  Kaikki versiot tai koontiversiot eivät Windows Bitlocker-asiakastukipalvelua. Tällä hetkellä Windows Versiot: Enterprise; Education, Mobile, Mobile Enterprise ja Professional (koontiversiosta 1809 alkaen) ovat tuettuja.




K: Jos laite on jo salattu BitLockerilla käyttämällä käyttöjärjestelmän salausmenetelmän ja salauksen oletusasetuksia (XTS-AES-128), käytännön käyttäminen eri asetuksilla käynnistää aseman uudelleensalauksen automaattisesti uusilla asetuksilla?

V: Ei. Jotta uudet salauksen asetukset voidaan ottaa käyttöön, aseman salaus on ensin purettava.

Huomautus Autopilotiin rekisteröidyissä laitteissa OOBE:n aikana suoritetaan automaattinen salaus vasta, kun Intune-käytäntö arvioidaan, jolloin käytäntöpohjaisia asetuksia voidaan käyttää käyttöjärjestelmän oletusasetusten asennuksilla




K Jos laite on salattu Intune-käytännön sovelluksen vuoksi, salauksen purkaminen poistetaan, kun tämä käytäntö poistetaan?

A: Salauskäytäntöjen poistaminen EI poista määritettyjen asemien salausta.




K: Miksi Intune-yhteensopivuuskäytäntö näyttää, että laitteessani ei ole BitLocker käytössä, mutta se on?

A: "Bitlocker käytössä" -asetus intunessa yhteensopivuuskäytäntö hyödyntää Windows Device Health Attestation (STATION) -asiakasohjelmaa. Tämä asiakas mittaa vain laitteen tilan käynnistyksen yhteydessä. Jos siis laitetta ei ole käynnistetty uudelleen bitlocker-salauksen jälkeen, SOVELLUKSE-asiakaspalvelu ei ilmoita bitlockerista aktiiviseksi.