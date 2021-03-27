---
title: Microsoft Edgen kehittyneen todentamisen käsitteet
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398556"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Microsoft Edgen kehittyneen todentamisen käsitteet

Seuraavassa ovat Microsoft Edgeen soveltuvat kehittyneen todentamisen käsitteet:

**Ennakoiva todennus**

Kun otat [ProactiveAuthEnabled-käytännön](https://go.microsoft.com/fwlink/?linkid=2134621) käyttöön, Microsoft Edge yrittää todentaa kirjautuneet käyttäjät ennakoivasti Microsoft-palvelujen kautta. Se tarkistaa säännöllisin väliajoin online-palvelun avulla päivitetyn luetteloluettelon, joka sisältää ennakoivaa todennusta koskevat määritykset.

Edut: Ennakoiva todentaminen mahdollistaa todennuksen tärkeimpiin palveluihin, kuten Officen Uusi välilehti -sivuun. Jos Bing-palvelua käytetään hakukoneena, ennakoiva todennus parantaa osoitepalkin suorituskykyä ja auttaa luomaan yrityksesi tarpeita mukautettuja hakutuloksia.

**Windows Hello CredUI NTLM-todennukseen**

Jos kertakirjautuminen (SSO) ei ole käytettävissä, kun sivusto yrittää kirjautua käyttäjääN NTLM- tai Negotiate-mekanismin avulla, käyttäjä voi jakaa käyttöjärjestelmän tunnistetiedot sivuston kanssa ja täyttää todennushaasteen Windows Hello Cred -käyttöliittymän avulla. Tämä kirjautumisvirta näkyy vain Windows 10:ssä ja vain käyttäjille, jotka eivät saa SSO-kirjautumista NTLM- tai Negotiate-haasteen aikana.

**Automaattinen kirjautuminen tallennettujen salasanojen avulla**

Käyttäjät, jotka tallentavat salasanoja Microsoft Edgeen, voivat ottaa käyttöön automaattisen kirjautumisen sivustoihin, joissa he ovat tallentaneet tunnistetietoja. Käyttäjät voivat ottaa tämän ominaisuuden käyttöön tai poistaa sen edge://settings/passwords, ja voit määrittää sen salasanojen hallinnan [käytännöistä.](https://go.microsoft.com/fwlink/?linkid=2134622)
