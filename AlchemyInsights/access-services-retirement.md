---
title: Access-palveluiden käytöstä poisto
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
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938692"
---
# <a name="access-services-retirement"></a>Access-palveluiden käytöstä poisto

Kuten alun perin ilmoitimme MC97576:ssa maaliskuussa 2017, ja viestintä jatkui viime vuoden aikana, Access Services käytöstä. Tämän prosessin seuraava vaihe on niiden Access-verkkotietokantojen poistaminen, jotka käyttävät SharePoint luetteloita pohjana olevana tietojen tallennuspaikkana.

**Miten tämä vaikuttaa minuun?**

Kesäkuusta 2019 alkaen Microsoft lopettaa uusien Access-tietokantojen luomisen SharePoint Onlinessa ja sulkee palvelun ja jäljellä olevat sovellukset huhtikuuhun 2020 mennessä.

**Miten voin valmistautua muutokseen?**

Suosittelemme, että luot siirtymäsuunnitelman organisaation Access-verkkotietokantoja varten. Järjestelmänvalvojat voivat [SharePoint Access-sovellusskannerin](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) avulla luettelon access-sovelluksista, joita sivustot käyttävät.

Access-verkkotietokantojen tietoja voi siirtää useilla eri tavoilla:

- Tuominen paikalliseen Access-tietokantaan (. ACCDB) tai Excel tiedostoon.
- Suosittelemme myös tutustumaan Microsoft PowerApps vaihtoehtoiseen käyttöympäristöön, jotta voit luoda koodikelvat yritysratkaisut verkko- ja mobiililaitteisiin.