---
title: Sähköpostiprofiilien käyttäminen Intunen kanssa
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
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554977"
---
# <a name="using-email-profiles-with-intune"></a>Sähköpostiprofiilien käyttäminen Intunen kanssa

Intune voidaan luoda ja ottaa käyttöön sähköpostiprofiileja natiivi (sisäänrakennettu) sähköpostiohjelma useilla laitealustoilla.

Lisätietoja joistakin sähköpostiprofiileihin liittyvistä rajoituksista, kuten olemassa olevien profiilien käsittelytapa ja sähköpostiprofiilien poistaminen, on [ohjeaiheessa Sähköpostiasetusten lisääminen laitteisiin Intune -toiminnolla](https://docs.microsoft.com/intune/email-settings-configure).

Lisätietoja sähköpostiprofiilien luomisesta kullekin laitealustalle on ohjeaiheessa:

[Android-laitteen asetukset sähköpostin, todennuksen ja synkronoinnin määrittämiseen Intuessa](https://docs.microsoft.com/intune/email-settings-android)  
[Sähköpostiasetusten lisääminen iOS- ja iPadOS-laitteille Microsoft Intutiin](https://docs.microsoft.com/intune/email-settings-ios)  
[Microsoft Intunen sähköpostiprofiilin asetukset Windows Phone 8.1 -laitteissa](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Sähköpostiprofiiliasetukset laitteille, joissa on Windows 10 Microsoft Intunen](https://docs.microsoft.com/intune/email-settings-windows-10)

**Yleinen synkronointiongelma**

**KNOX Android-sähköpostiprofiilissa estää käyttäjän yhteystietojen, kalenterin ja tehtävien synkronoinnin käyttäjän laitteisiin.**

Knox Android KNOX -sähköpostiprofiilissa tarjoaa järjestelmänvalvojalle mahdollisuuden päättää, mitkä sisältötyypit synkronoidaan laitteeseen asettamalla kukin käyttöön.

Jos jonkin sisältötyypin asetuksena on **Ei määritetty** (oletusasetus), kyseistä sisältötyyppiä ei synkronoida automaattisesti. Käyttäjä saattaa ottaa haluamasi sisältötyypin käyttöön suoraan laitteeseen manuaalisesti, mutta Intune-käytäntöasetus korvaa kyseisen kokoonpanon ja kyseisen sisältötyypin synkronointi pysähtyy.

