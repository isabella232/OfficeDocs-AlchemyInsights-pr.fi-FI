---
title: Teams 4c7 -virhe
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049305"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7-virhe Microsoft Teams

Tämä virhe ilmenee, koska Microsoft Teams edellyttää lomakkeiden todennusta. Kun otat Active Directory Federation Servicesin (AD FS) käyttöön, lomakkeiden todennus ei ole oletusarvoisesti käytössä intranetissä. Jos Windows integroitu todennus epäonnistuu, sinua pyydetään kirjautumaan sisään käyttämällä Forms-todennusta.

Voit ratkaista tämän ongelman käyttäen AD FS Microsoft Management Console (MMC) -laajennusta tietokoneessa, jossa on paikallinen Active Directory -versio, käyttäen lomakkeiden todennusta. Voit tehdä tämän seuraavasti: 

1. Valitse siirtymisruudussa **Todennuskäytännöt.**
2. Valitse **tietoruudun** Toiminnot-kohdassa Muokkaa **yleisessä ensisijaisessa todentamisessa**.
3. Valitse **Intranet-välilehdessä** **Lomakkeiden todennus**.
4. Valitse **OK** (tai **Käytä).**