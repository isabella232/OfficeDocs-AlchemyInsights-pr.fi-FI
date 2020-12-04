---
title: Windows 10-laitteiden määrittäminen Microsoft Intune-tieto turva perusaikataulujen avulla
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
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573400"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Windows 10-laitteiden määrittäminen Microsoft Intune-tieto turva perusaikataulujen avulla

Intune-suojaus perusaikataulujen avulla voit suojata käyttäjiä ja laitteita. Tieto turvan perusaikataulut ovat Windowsin asetukset valmiiksi määritetyt ryhmät, joita käytetään tunnettujen tieto turva ryhmien suosittelemien asetus ryhmien ja oletus arvojen käyttöön. Luomalla Intune-tieto turvan Perusprofiilin luot mallin, joka koostuu useista laite määritys profiileista.

Kun otat käyttöön tieto turvan perusviivat käyttäjien tai laitteiden ryhmille, asetukset otetaan käyttöön laitteissa, jotka toimivat Windows 10: ssä tai sitä uudemmissa versioissa. Esimerkiksi MDM-tieto turvan perusaikataulu (1) mahdollistaa siirrettävien asemien BitLocker-Sala uksen, (2) edellyttää laitteen lukituksen poistamiseen ja (3) poistaa perustodennuksen käytöstä. Kun oletus arvo ei toimi ympäristössäsi, Mukauta perusviivaa ja ota käyttöön tarvitsemasi asetukset.

Tieto turvan perusaikataulujen avulla voit myös määrittää end-to-end-suojatun työn kulun Microsoft 365. Seuraavista eduista on hyötyä:

- Tieto turvan perusaikataulu sisältää parhaita käytäntöjä ja suosituksia, jotka vaikuttavat tieto turvaan. Koska Intune-kumppanit käyttävät Windowsin tieto turva tiimiä, joka luo perusaikatauluja ryhmä käytännöille, nämä suositukset perustuvat kiinteään ohja ukseen ja laajaan kokemukseen.
- Jos olet uusi Intune-käyttäjä ja olet epävarma aloitus paikasta, voit luoda ja ottaa käyttöön suojatun profiilin nopeasti luomalla suojaus perusaikataulujen avulla.
- Jos käytät tällä hetkellä ryhmä käytäntöä, siirtyminen Intune-järjestelmään hallinta tarkoituksissa on paljon helpompaa, koska ne on luotu Intune-käyttöön ja ne sisältävät hallinnan huippu ominaisuudet.

Lisä tietoja on artikkelissa [Windowsin tieto turvan perusviivat](https://go.microsoft.com/fwlink/?linkid=2141503) ja [mobiililaitteiden hallinta](https://go.microsoft.com/fwlink/?linkid=2141701).