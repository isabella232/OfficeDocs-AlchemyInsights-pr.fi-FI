---
title: Sähköpostiprofiilien käyttäminen Intunen kanssa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919420"
---
# <a name="using-email-profiles-with-intune"></a>Sähköpostiprofiilien käyttäminen Intunen kanssa

Intunen avulla voidaan luoda ja ottaa käyttöön sähköpostiprofiileja alkuperäisessä (sisäisessä) sähköpostiohjelmassa useissa laiteympäristöissä.

Lisätietoja sähköpostiprofiileihin liittyvistä rajoituksista, kuten siitä, miten olemassa olevia profiileja käsitellään ja miten sähköpostiprofiilit poistetaan, on kohdassa Sähköpostiasetusten lisääminen [laitteisiin Intunen avulla.](https://docs.microsoft.com/intune/email-settings-configure)

Lisätietoja sähköpostiprofiilien luostasta kullekin laiteympäristölle on kohdassa:

[Android-laitteen asetukset sähköpostin, todennuksen ja synkronoinnin määrittämiseksi Intunessa](https://docs.microsoft.com/intune/email-settings-android)  
[iOS- ja iPadOS-laitteiden sähköpostiasetusten lisääminen Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Sähköpostiprofiilin asetukset Microsoft Intune 8.1-Windows Phone laitteissa](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Sähköpostiprofiilin asetukset Windows 10 Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Yleinen synkronointiongelma**

**Androidin sähköpostiprofiilin KNOX estää yhteystietojen, kalenterin ja tehtävien synkronoinnin käyttäjien laitteisiin.**

Androidin KNOX-sähköpostiprofiilin avulla järjestelmänvalvoja voi päättää, mitkä sisältötyypit synkronoidaan laitteeseen määrittämällä ne käyttöön.

Jos jonkin sisältötyypin asetuksena on  Ei määritetty (oletus), tätä sisältötyyppiä ei synkronoida automaattisesti. Käyttäjä voi ottaa haluamasi sisältötyypin käyttöön suoraan laitteessa manuaalisesti, mutta tämä määritys korvataan Intune-käytäntöasetuksella ja tämän sisältötyypin synkronointi loppuu.

