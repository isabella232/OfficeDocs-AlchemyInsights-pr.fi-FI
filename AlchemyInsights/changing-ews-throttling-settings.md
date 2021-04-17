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
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818033"
---
# <a name="changing-ews-throttling-settings"></a>Muutetaan EWS-rajoitusasetuksia

Suorita automaattinen testimme, jonka avulla voit muuttaa EWS-rajoituskäytäntöä siirron ajaksi. Huomaa, että testin suorituksenkin jälkeen, EWS-tuonnit on silti rajoitettu 150 megatavuun 5 minuutin sisällä postilaatikkoa kohti. Jos haluat saavuttaa korkeammat siirtonopeudet, siirrä useampia käyttäjiä samanaikaisesti.

Huomaa, että EWS-rajoituskäytännön muutoksilla ei ole vaikutusta seuraaviin siirtotyyppeihin (Microsoft-työkaluja käytettäessä): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Yleinen kansio tai PST-tuontipalvelu.