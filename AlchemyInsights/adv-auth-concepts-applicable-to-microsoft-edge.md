---
title: Edistyneet todentamisen käsitteet Microsoft Edge
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
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934362"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Edistyneet todentamisen käsitteet Microsoft Edge

Seuraavassa ovat todennuskäsitteet, jotka koskevat Microsoft Edge:

**Ennakoiva todennus**

Kun otat [ProactiveAuthEnabled-käytännön](https://go.microsoft.com/fwlink/?linkid=2134621) käyttöön, Microsoft Edge yrittää aktiivisesti todentaa kirjautuneet käyttäjät Microsoft-palvelut. Se tarkistaa säännöllisin väliajoin online-palvelun avulla päivitetyn kokoonpanon, joka sisältää ennakoivaa todentamista koskevat määritykset.

Edut: Ennakoiva todentaminen mahdollistaa todennuksen avainpalveluihin, kuten Office uusi välilehti -sivuun. Jos Bing hakukoneena, ennakoiva todennus parantaa osoitepalkin suorituskykyä ja auttaa luomaan yrityksesi tarpeita mukautettuja hakutuloksia.

**Windows Hello NTLM-todennuksen CredUI**

Jos kertakirjautuminen (SSO) ei ole käytettävissä, kun sivusto yrittää kirjautua käyttäjälle NTLM- tai Negotiate-mekanismin avulla, käyttäjä voi jakaa käyttöjärjestelmän tunnistetiedot sivuston kanssa ja täyttää todennushaasteen Windows Hello Cred -käyttöliittymän avulla. Kirjautumisen kulku näkyy vain Windows 10 käyttäjille, jotka eivät saa SSO-kirjautumista NTLM- tai Negotiate-haasteen aikana.

**Automaattinen kirjautuminen tallennettujen salasanojen avulla**

Käyttäjät, jotka tallentavat salasanoja Microsoft Edge voivat ottaa käyttöön automaattisen kirjautumisen sivustoihin, joissa he ovat tallentaneet tunnistetiedot. Käyttäjät voivat ottaa tämän toiminnon käyttöön tai poistaa sen edge://settings/passwords ja voit määrittää sen salasanojen hallinnan [käytännöistä.](https://go.microsoft.com/fwlink/?linkid=2134622)
