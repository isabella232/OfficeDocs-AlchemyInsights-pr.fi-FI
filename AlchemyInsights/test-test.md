---
title: SharePoint Online Term Storesta puuttuvat termit
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766850"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Bitlocker-salauksen ottaminen käyttöön Intunen avulla

Intune Endpoint Protection Policy -käytännön avulla voit määrittää Boitlocker-salausasetukset Windows-laitteille kohdassa : Windows10 (ja uudemmat) -asetukset laitteiden suojaamiseksi Intunen avulla

Sinun tulisi olla tietoinen siitä, että monet uudemmat laitteet, joissa on Windows 10, tukevat automaattista bitlocker-salausta, joka käynnistyy ilman MDM-käytännön soveltamista. Tämä saattaa vaikuttaa käytännön soveltamiseen, jos muut kuin oletusasetukset on määritetty. Lisätietoja on usein kysytyissä kysymyksissä.


USEIN  KYSYTYT KYSYMYKSET Q: Mitkä Windows-versiot tukevat laitesalausta päätepisteen suojauskäytännön avulla?
 V: Intune Endpoint Protection Policy -käytännön asetukset otetaan käyttöön Bitlockerin CSP-järjestelmän avulla.Kaikki versiot tai Windows-koontiversiot eivät tue Bitlockerin CSP:tä. 
      Tällä hetkellä Windows-versiot: Enterprise; Koulutus, Mobile, Mobile Enterprise ja Professional (alkaen rakentaa 1809 lähtien) ovat tuettuja.




K: Jos laite on jo salattu Bitlockerilla käyttäen käyttöjärjestelmän salausmenetelmän ja salakirjoituksen voimakkuutta (XTS-AES-128), sovelletaankäytäntöä, jolla on eri asetukset, käynnistämään aseman uudelleensalauksen automaattisesti uusilla asetuksilla?

V: Ei. Uusien salausasetusten ottamiseksi käyttöön asema on ensin purettava.

Huomautus Autopilotilla rekisteröitävien laitteiden automaattinen salaus, joka tapahtuu OOBE:n aikana, ei käynnisty, ennen kuin Intune-käytäntö on arvioitu, jolloin käytäntöpohjaisia asetuksia voidaan käyttää käyttöjärjestelmän oletusasetusten sijasta




Q Jos laite on salattu Intune-käytännön soveltamisen seurauksena, puretaanko sen salaus, kun kyseinen käytäntö poistetaan?

V: Salaukseen liittyvän käytännön poistaminen EI johda määritettyjen asemien salauksen purkamiseen.




K: Miksi intune Compliance -käytäntö osoittaa, että laitteessani ei ole Bitlocker-käyttölaitetta, mutta se on?

V: Intune-yhteensopivuuskäytännön Bitlocker-asetus käyttää Windows Device Health Attestation (DHA) -asiakasta. Tämä asiakas mittaa laitteen tilaa vain käynnistyksen aikana. Jos laitetta ei ole käynnistetty uudelleen bitlocker-salauksen valmistuttua, DHA-asiakaspalvelu ei ilmoita bitlockerista aktiiviseksi.