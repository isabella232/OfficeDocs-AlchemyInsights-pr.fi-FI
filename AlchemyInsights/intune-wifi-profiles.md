---
title: Intune Wi-Fi-profiilit
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555006"
---
# <a name="intune-wi-fi-profiles"></a>Intune Wi-Fi-profiilit

Wi-Fi-yhteyden onnistunut käyttöönotto MDM-asiakkaille riippuu oikein käyttöön otetusta profiilista, joka vastaa yrityksen Wi-Fi-infrastruktuurin vaatimuksia. Jos haluat tarkastella tutkimiesi asiakasympäristöjen asetuksia, katso: 

[Wi-Fi-asetusten lisääminen laitteille, joissa on Android Microsoft Intunen](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Wi-Fi-asetusten lisääminen Android Enterprise -omistautuneille ja täysin hallituille laitteille Microsoft Intunen avulla](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Wi-Fi-asetusten lisääminen iOS- ja iPadOS-laitteille Microsoft Intutiin](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Wi-Fi-asetusten lisääminen Windows 10:lle ja uudemmillesi laitteille Intutiin](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Wi-Fi-asetusten tuominen Windows-laitteille Intuessa](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Yleisiä ongelmia**

**Otan käyttöön Wi-Fi-profiilin, joka on riippuvainen Wi-Fi-profiilissa määritetystä käyttöönottannista varmenteesta. Määritysprofiileissa näkyy kuitenkin virheen tila.**

Tarkista, että laitteesi on saanut varmenteen.

1. Valitse Intunessa **Kaikki laitteet** ja valitse laite > **Laiteasetukset**.

2. Tarkista, että kaikki odotetut profiilit on lueteltu ja että ne ovat onnistuneessa tilassa.

3. Jos sinulla on Android-profiilissa välivarmenteita varmenneketjussasi, varmista, että ne on otettu käyttöön Android-laitteissa.

    Voit tarkistaa varmenteen tilan siirtymällä **kohtaan Laitteen**  >  **määritysprofiilit**  >  **Android intermediate CA**  >  **Properties**  >  **Trusted Certificate**.

Jos virheet jatkuvat, tutustu toimintosarjoihin ja vianmääritysosioihin. Lisätietoja on [ohjeaiheessa Scep-varmenneprofiilien vianmääritys Microsoft Intunen avulla](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Olen ottanut Wi-Fi-profiilin käyttöön laitteessa. Intune näyttää, että se onnistui, mutta laite ei muodosta yhteyttä Wi-Fi-verkkoon.**

Onnistunut tila tarkoittaa, että Intune on ottanut profiilin onnistuneesti käyttöön määritetyllä tavalla. Nämä määritykset eivät kuitenkaan välttämättä vastaa verkko- ja/tai todennusvaatimuksia. Lisätietoja yhteyden yrittämisestä on infrastruktuuri- ja todennuspalvelun lokeissa (Wi-Fi-tukiaseman ohjaimessa ja NPS/Radius-palvelimessa). Saatat joutua työskentelemään verkkoinfrastruktuuritiimin tai kolmannen osapuolen Wi-Fi-toimittajan kanssa lokien keräämiseksi ja tarkistamiseksi.