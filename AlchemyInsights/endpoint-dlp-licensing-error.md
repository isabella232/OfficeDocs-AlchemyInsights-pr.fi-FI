---
title: Päätepisteen DLP-käyttöoikeusvirhe
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
ms.openlocfilehash: 1e242abe18717e5ef64d6f067ab3ec6fa8833cb672dd21c85e577ce640240ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090133"
---
# <a name="endpoint-dlp-licensing-error"></a>Päätepisteen DLP-käyttöoikeusvirhe

Kun yrität määrittää DLP-päätepistettä, saat seuraavan virheilmoituksen:

`Your organization is missing the licenses required to manage these devices`.

Varmista, että käytössäsi on jokin seuraavista tilauksia tai lisätilauksia:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 yhteensopivuus
- Microsoft 365 A5 yhteensopivuus
- Microsoft 365 E5 ja hallinta
- Microsoft 365 A5 ja hallinta

> [!NOTE]
> Tämä ei toimi käyttöoikeusyhdistelmissä, kuten Win E5 + O365 E5 + EMS E5. Sinulla on oltava täysin M365 E5 -käyttöoikeus, jotta voit määrittää tämän ominaisuuden.

Lisätietoja Endpoint DLP -käyttöoikeuksista on kohdassa [Endpoint DLP Licensing (DLP-käyttöoikeudet).](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
