---
title: Perusaikataulujen Microsoft Intune määrittäminen laitteiden Windows 10 perusaikataulujen avulla
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 911c6b1860e4f44e6d88897f73173cdd11060562
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331982"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Perusaikataulujen Microsoft Intune määrittäminen laitteiden Windows 10 perusaikataulujen avulla

Intune-suojauksen perusaikataulut auttavat suojaamaan käyttäjiä ja laitteita. Suojauksen perusaikataulut ovat Windows määritettyjä ryhmiä, joiden avulla käytetään tunnettua joukkoa asetuksia ja oletusarvoja, joita asianomaiset suojausryhmät suosittelevat. Luomalla suojauksen perusaikataulun profiilin Intunessa voit luoda mallin, joka koostuu useista laitemääritysprofiileista.

Kun otat käyttöön suojauksen perusaikataulut käyttäjä- tai laiteryhmissä, asetukset otetaan käyttöön laitteissa, jotka suoritetaan Windows 10 uudemmassa. Esimerkiksi Microsoftin mobiililaitteiden hallinnan perussuojaus ottaa BitLockerin automaattisesti käyttöön siirrettävissä asemissa, vaatii salasanan laitteen lukituksen poistamiseen ja poistaa perustodennuksen käytöstä. Jos oletusarvo ei toimi ympäristössäsi, voit mukauttaa perusaikataulua tarvitsemallasi asetuksilla.

Suojauksen perusaikataulut auttavat myös luomaan lopusta loppuun suojatun työnkulun Microsoft 365. Suojauksen perusaikataulu sisältää parhaat käytännöt ja suojausta koskevat asetukset. Intune kumppanit Windows kanssa, joka luo perusaikatauluja ryhmäkäytäntöjä varten, joten nämä suositukset perustuvat vankkaon ohjeeseen ja laajaan käyttökokemukseen.

Jos et ole ennen luonut Intunea etkä tiedä, mistä aloittaa, suojauksen perusaikataulujen avulla voit luoda ja ottaa käyttöön suojatun profiilin nopeasti. Jos käytät tällä hetkellä ryhmäkäytäntöä, siirtyminen Intuneen hallintatarkoituksiin on huomattavasti helpompaa suojauksen perusaikataulujen avulla, koska ne sisältyvät Intuneen ja sisältävät huipputason hallintaominaisuuksia.

Lisätietoja on ohjeaiheessa Windows [perusaikataulut ja](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) [mobiililaitteiden hallinta.](https://docs.microsoft.com/windows/client-management/mdm/)

