---
title: SharePoint Suunnittelutyökalun yhteysongelmat
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942022"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Suunnittelutyökalun yhteysongelmat 

Jos SharePoint suunnittelutyökalulla on yhteysongelmia SharePoint sivustoihin, kokeile seuraavia yleisiä ratkaisuja.

Vaihe 1: varmista, että SharePoint Designer 2013:ssa on [päivitetty SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ja SharePoint Designer [2013:n 2. elokuuta 2016 -päivitys.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



Vaihe 2: Tyhjennä paikalliset välimuistitiedostot:

1. Sulje SharePoint Designer 2013.

2. Poista paikallisessa tietokoneessa kaikki seuraavien kansioiden tiedostot.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Avaa SharePoint Designer 2013 ja katso, toimiiko se kirjoittamalla tili uudelleen.

Vaihe 3: [Modernin todentamisen ottaminen käyttöön Office 2013:ssa Windows laitteissa.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Vaihe 4: Järjestelmänvalvojien on sallittava mukautettu komentosarja SharePoint hallintakeskuksen asetuksissa, jotta SharePoint suunnittelutyökalun yhteys.  Lisätietoja [on kohdassa Mukautetun komentosarjan salliminen](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) tai estäminen.


