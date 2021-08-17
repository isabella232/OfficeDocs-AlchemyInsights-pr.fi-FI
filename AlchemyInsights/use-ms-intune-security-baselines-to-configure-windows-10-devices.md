---
title: Perusaikataulujen Microsoft Intune määrittäminen laitteiden Windows 10 perusaikataulujen avulla
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104341"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Perusaikataulujen Microsoft Intune määrittäminen laitteiden Windows 10 perusaikataulujen avulla

Intune-suojauksen perusaikataulut auttavat suojaamaan käyttäjiä ja laitteita. Suojauksen perusaikataulut Windows ovat valmiiksi määritettyjä ryhmiä, joiden avulla käytetään tunnettua joukkoa asetuksia ja oletusarvoja, joita asianomaiset suojausryhmät suosittelevat. Luomalla suojauksen perusaikataulun profiilin Intunessa voit luoda mallin, joka koostuu useista laitemääritysprofiileista.

Kun otat käyttöön suojauksen perusaikataulut käyttäjä- tai laiteryhmissä, asetukset otetaan käyttöön laitteissa, jotka suoritetaan Windows 10 uudemmassa. Esimerkiksi MDM Security Baseline ottaa BitLockerin käyttöön siirrettävissä asemissa automaattisesti (1), (2) edellyttää salasanan laitteen lukituksen avaamista varten ja (3) poistaa perustodennuksen käytöstä. Jos oletusarvo ei toimi ympäristössäsi, mukauta perusaikataulua tarvitsemallasi asetuksilla.

Suojauksen perusaikataulut auttavat myös luomaan lopusta loppuun suojatun työnkulun Microsoft 365. Seuraavassa on joitakin etuja:

- Suojauksen perusaikataulu sisältää parhaat käytännöt ja suojausta koskevat asetukset. Koska Intune on työryhmän Windows, joka luo perusaikatauluja ryhmäkäytäntöjä varten, nämä suositukset perustuvat vankkaon ohjeeseen ja laajaan käyttökokemukseen.
- Jos et ole ennen luonut Intunea etkä tiedä, mistä aloittaa, suojausaikataulujen avulla voit luoda ja ottaa käyttöön suojatun profiilin nopeasti.
- Jos käytät tällä hetkellä ryhmäkäytäntöä, siirtyminen Intuneen hallintatarkoituksiin on huomattavasti helpompaa suojauksen perusaikataulujen avulla, koska ne sisältyvät Intuneen ja sisältävät hallinnan huippuominaisuuksia.

Lisätietoja on ohjeaiheessa Windows [perusaikataulut ja](https://go.microsoft.com/fwlink/?linkid=2141503) [mobiililaitteiden hallinta.](https://go.microsoft.com/fwlink/?linkid=2141701)