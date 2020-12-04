---
title: Microsoft Edgeen sovellettavat kehittyneet todennus konseptit
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573395"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Microsoft Edgeen sovellettavat kehittyneet todennus konseptit

Seuraavat ovat Microsoft Edgeen sovellettavat kehittyneet todennus konseptit:

**Ennakoiva todentaminen**

Kun otat [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) -käytännöt käyttöön, Microsoft Edge yrittää todentaa kirjautuneet käyttäjät ennakoivasti Microsoft-palveluiden kautta. Säännöllisin väli ajoin se käyttää online-palvelua tarkistamaan päivitetyn luettelon, joka sisältää ennakoivan todennuksen määrityksen.

Edut: Ennakoiva todentaminen mahdollistaa todennuksen keskeisiin palveluihin, kuten Officen uusi väli lehti-sivulle. Jos haku kone käyttää Bing-palvelua, ennakoiva todentaminen parantaa osoite rivin suoritus kykyä ja auttaa luomaan yrityksesi tarpeisiin mukautettuja haku tuloksia.

**Windows Hello CredUI NTLM-todennusta varten**

Jos kertakirjautuminen (SSO) ei ole käytettävissä, kun sivusto yrittää kirja utua käyttäjään NTLM-tai neuvottelu mekanismin kautta, tämän ominaisuuden avulla käyttäjä voi jakaa käyttö järjestelmän tunniste tiedot sivuston kanssa ja täyttää todennus haasteen Windows Hello Cred UI-sovelluksen avulla. Tämä kirjautumisvuo näkyy vain Windows 10: ssä ja vain niille käyttäjille, jotka eivät saa kertakirjautumista NTLM-tai neuvottelu haasteen aikana.

**Automaattisen kirjautumisen käyttäminen tallennettujen Sala sanojen avulla**

Käyttäjät, jotka tallentavat Sala sanat Microsoft Edgessä, voivat ottaa automaattisen kirjautumisen käyttöön sivustoissa, joihin heillä on tallennettuja tunniste tietoja. Käyttäjät voivat ottaa tämän toiminnon käyttöön tai poistaa sen käytöstä edge://settings/passwords-sovelluksessa, ja voit määrittää sen [Sala sanan hallintaan](https://go.microsoft.com/fwlink/?linkid=2134622) .
