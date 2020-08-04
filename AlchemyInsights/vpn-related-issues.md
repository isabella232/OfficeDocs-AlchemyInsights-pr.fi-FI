---
title: VPN:ään liittyvät ongelmat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554969"
---
# <a name="vpn-related-issues"></a>VPN:ään liittyvät ongelmat

VPN-yhteyden onnistunut käyttöönotto MDM-asiakkaille riippuu käyttöönotetusta profiilista, joka vastaa oikein VPN-infrastruktuurin vaatimuksia. Asianmukaiset asetukset tutkimillesi asiakasalustoille ovat seuraavissa ohjeissa: 

[Windows 10:n ja Windowsin hologrammilaitteen asetukset VPN-yhteyksien lisäämiseksi Intunen avulla](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[VPN-asetusten lisääminen iOS- ja iPadOS-laitteisiin Microsoft Intuessa](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Android-laitteen asetukset VPN:n määrittämiseen Intunessa](https://docs.microsoft.com/intune/vpn-settings-android)  
[VPN-asetusten lisääminen macOS-laitteisiin Microsoft Intunen avulla](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Jos VPN-profiilisi käyttää varmennepohjaista todennusta, varmista, että VPN-profiiliin linkitetyt päävarmenteen ja asiakkaan todennusvarmenneprofiilit otetaan käyttöön onnistuneesti.

**Yleisiä ongelmia**

**Otin VPN-profiilin käyttöön laitteessa. Intune näyttää onnistuneen, mutta laite ei muodosta yhteyttä VPN:ään.**

Onnistunut tila tarkoittaa, että Intune on ottanut profiilin onnistuneesti käyttöön määritetyllä tavalla. Nämä määritykset eivät kuitenkaan välttämättä vastaa verkko- ja/tai todennusvaatimuksia. Lisätietoja yhteyden yrittämisestä on infrastruktuuri- ja todennuspalvelun lokeissa (VPN-palvelimessa ja NPS/Radius-palvelimessa). Sinun on ehkä työskenneltävä verkkoinfrastruktuuritiimisi tai kolmannen osapuolen VPN-toimittajan kanssa, jotta voit kerätä ja tarkastella lokeja.

**Kun määritän mukautetun VPN:n iOS:lle, sovelluskohtainen VPN-ominaisuus ei ole käytettävissä.**

Intunen iOS-laitteiden sovelluskohtainen VPN on tällä hetkellä saatavilla tietylle palveluntarjoajien ja kumppanien luettelolle, jonka on myös täytettävä varmenteen edellytykset ennen sovelluksenkohtaisen VPN:n määrittämistä. Lisätietoja on kohdassa [Sovelluksen virtuaalisen yksityisverkon (VPN) määrittäminen iOS/iPadOS-laitteille Intuessa](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Lisätietoja kaikista Intunen VPN-yhteystyypeistä on ohjeaiheessa [VPN-profiilien luominen vpn-palvelimiin yhdistämistä varten Intuessa](https://docs.microsoft.com/intune/vpn-settings-configure).  

**iOS On-Demand VPN ei käynnisty, kun määritettyä toimialuetta käytetään**

Voit testata automaattisia VPN-asetuksia määrittämällä seuraavat arvot:

Haluan tehdä seuraavat toimet: **Arvioi jokainen yhteysyritys** 

Valitse, haluatko muodostaa yhteyden: **Yhdistä tarvittaessa**

Kun käyttäjät voivat käyttää näitä toimialueita: **target** *kohdetoimialueen nimi*

Jos edellä mainittu kokoonpano ei onnistu, lisää seuraava elementti:

Kun tätä URL-osoitetta ei saada, pakota vpn: **BADURL**