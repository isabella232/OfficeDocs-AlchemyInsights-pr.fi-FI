---
title: Siirtosääntöjen ratkaiseminen
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746739"
---
# <a name="fix-transport-rules"></a>Siirtosääntöjen ratkaiseminen

Tämä sanoma vaikuttaa mukautettuun postinkulkusääntöön. Voit tarkistaa täsmällisen säännön seuraavasti:

1. Huomaa lähetyksen tuloksissa **Lisätietoja-kohdassa** **GUID-tunnus** tai **käytännön nimi.**
2. Käynnistä Exchange-hallintaliittymä. Lisätietoja on ohjeaiheessa [Exchange-hallintaliittymän avaaminen.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Suorita tämä komento (käyttämällä lähetyksen  **GUID-tunnusta): Get-TransportRule -identity "GUID" | fl * Description***
4. Tarkista kuvaus, jotta näet määritetyt ehdot, joihin viesti vaikuttaa.

Lisätietoja on kohdassa [Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)
