---
title: Siirtosääntöjen korjaukset
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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694150"
---
# <a name="fix-transport-rules"></a>Siirtosääntöjen korjaukset

Tämä sanoma vaikuttaa mukautettuun postinkulkusääntöön. Voit tarkistaa täsmällisen säännön seuraavasti:

1. Merkitse muistiin lähetyksen tulosten **Lisätiedot-kohdassa** **GUID-tunnus** tai **käytännön nimi.**
2. Käynnistä Exchange-hallintaliittymä. Lisätietoja on ohjeaiheessa [Exchange-hallintaliittymän avaaminen.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Suorita tämä komento (käyttämällä lähetyksen  **GUID-tunnusta): Get-TransportRule -identity "GUID" | fl * Description***
4. Tarkista kuvaus, jotta näet määritetyt ehdot, jotka vaikuttavat viestiin.

Lisätietoja on kohdassa [Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)
