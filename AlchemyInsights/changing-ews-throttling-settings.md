---
title: Muutetaan EWS-rajoitusasetuksia
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075894"
---
# <a name="changing-ews-throttling-settings"></a>Muutetaan EWS-rajoitusasetuksia

Suorita automaattinen testimme, jonka avulla voit muuttaa EWS-rajoituskäytäntöä siirron ajaksi. Huomaa, että suorituksen jälkeen, EWS-tuonnit on silti rajoitettu 150 megatavuun 5 minuutin sisällä per postilaatikko. Jos haluat saavuttaa korkeammat siirtonopeudet, siirrä useampia käyttäjiä samanaikaisesti.

Huomaa, että EWS-rajoituskäytännön muutoksilla ei ole vaikutusta seuraaviin siirtotyyppeihin (Microsoft-työkaluja käytettäessä): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Yleinen kansio tai PST-tuontipalvelu.