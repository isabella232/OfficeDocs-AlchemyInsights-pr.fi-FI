---
title: Palveluiden käytön keskeytys
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698679"
---
# <a name="access-services-retirement"></a>Palveluiden käytön keskeytys

Kuten alun perin ilmoitettiin MC97576, maaliskuussa 2017 ja jatkoi viestintää kuluneen vuoden aikana, palvelu on poistettu käytöstä. Tämän prosessin seuraava vaihe on sellaisten Accessia käyttävien verkko tieto kantojen poistaminen, jotka käyttävät SharePoint-luetteloita pohjana olevien tietojen tallentamiseen.

**Miten tämä vaikuttaa minuun?**

Kesä kuun 2019 jälkeen lopetamme uusien tieto kantojen luomisen SharePoint Onlinessa ja suljet palvelun ja kaikki jäljellä olevat sovellukset huhtikuuhun 2020 mennessä.

**Mitä minun on tehtävä tämän muutoksen valmistelemiseksi?**

Kehotamme sinua luomaan siirtymäsuunnitelmat organisaation verkko tieto kantoja varten. Järjestelmänvalvojat voivat käyttää [SharePoint-sovelluksen sovellus skanneria](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) , joka hankkii luettelon käyttö oikeus sovelluksista, joita sivustot käyttävät.

Voit siirtää Accessia koskevia verkko tieto kanta tietoja usealla eri tavalla:

- Tuominen paikalliseen tieto kantaan (. ACCDB) tai Excel-tiedostoon.
- Suosittelemme myös tutustumaan Microsoft PowerApps-sovelluksiin vaihtoehtoisena ympäristönä, jotta voit luoda ei-koodi ratkaisuja verkko-ja mobiililaitteisiin.