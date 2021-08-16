---
title: Muutetaan EWS-rajoitusasetuksia
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968374"
---
# <a name="changing-ews-throttling-settings"></a>Muutetaan EWS-rajoitusasetuksia

Suorita automaattinen testimme, jonka avulla voit muuttaa EWS-rajoituskäytäntöä siirron ajaksi. Huomaa, että testin suorituksenkin jälkeen, EWS-tuonnit on silti rajoitettu 150 megatavuun 5 minuutin sisällä postilaatikkoa kohti. Jos haluat saavuttaa korkeammat siirtonopeudet, siirrä useampia käyttäjiä samanaikaisesti.

Huomaa, että EWS-rajoituskäytännön muutoksilla ei ole vaikutusta seuraaviin siirtotyyppeihin (Microsoft-työkaluja käytettäessä): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Yleinen kansio tai PST-tuontipalvelu.