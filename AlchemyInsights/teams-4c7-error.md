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
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786666"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7-virhe Microsoft Teamsissa

Tämä virhe ilmenee, koska Microsoft Teams edellyttää Forms-todennusta. Kun otat Active Directory Federation Servicesin (AD FS) käyttöön, lomakkeiden todennus ei ole oletusarvoisesti käytössä intranetissä. Jos Windows Integrated Authentication epäonnistuu, sinua pyydetään kirjautumaan sisään käyttämällä Forms-todennusta.

Voit ratkaista tämän ongelman käyttäen AD FS Microsoft Management Console (MMC) -laajennusta tietokoneessa, jossa on paikallinen Active Directory -versio, käyttäen lomakkeiden todennusta. Voit tehdä tämän seuraavasti: 

1. Valitse siirtymisruudussa **Todennuskäytännöt.**
2. Valitse **tietoruudun** Toiminnot-kohdassa Muokkaa **yleisessä ensisijaisessa todentamisessa**.
3. Valitse **Intranet-välilehdessä** **Lomakkeiden todennus**.
4. Valitse **OK** (tai **Käytä).**