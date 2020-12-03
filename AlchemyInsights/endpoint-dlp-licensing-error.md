---
title: Pääte pisteen DLP-käyttö oikeus virhe
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564483"
---
# <a name="endpoint-dlp-licensing-error"></a>Pääte pisteen DLP-käyttö oikeus virhe

Kun yrität määrittää pääte pisteen DLP, jos saat seuraavan virhe ilmoituksen:

`Your organization is missing the licenses required to manage these devices`.

Varmista, että sinulla on jokin seuraavista paketeista tai lisä osista:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5-yhteensopivuus
- Microsoft 365 A5-yhteensopivuus
- Microsoft 365 E5 tietojen suojaaminen ja hallinta
- Microsoft 365 A5-tieto turva ja-hallinta

> [!NOTE]
> Tämä ei toimi käyttö oikeus yhdistelmissä, kuten: Win E5 + O365 E5 + EMS E5. Sinulla on oltava puhdas M365 E5-käyttö oikeus, jotta voit määrittää tämän ominaisuuden.

Lisä tietoja pääte pisteiden DLP-käyttö oikeus tiedoista on kohdassa [Endpoint DLP Licensing.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
