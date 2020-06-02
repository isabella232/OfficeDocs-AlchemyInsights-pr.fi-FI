---
title: SharePoint Designerin yhteysongelmat
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511541"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designerin yhteysongelmat 

Jos SharePoint Designerilla on yhteysongelmia SharePoint-sivustoihin, kokeile seuraavia yleisiä ratkaisuja.

Vaihe 1: Varmista, että SharePoint Designer 2013:n [sharepoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ja [SharePoint Designer 2013:n 2.8.2016 -päivitys](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)päivittyvät.



Vaihe 2: Tyhjennä paikalliset välimuistitiedostot:

1. Sulje SharePoint Designer 2013.

2. Poista paikallisessa tietokoneessa kaikki seuraavista kansioista löydetyt tiedostot.

    - %APPDATA%\Microsoft\Web-palvelinlaajennukset\Välimuisti
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Avaa SharePoint Designer 2013 ja anna tili uudelleen, jotta näet toimiiko se.

Vaihe 3: [Ota office 2013:n nykyaikainen todennus käyttöön Windows-laitteissa](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Vaihe 4: Järjestelmänvalvojien on **sallittava mukautettu komentosarja** SharePoint-hallintakeskuksen asetuksissa, jotta SharePoint Designer -yhteys voidaan muodostaa. Lisätietoja [on ohjeaiheessa Mukautetun komentosarjan salliminen tai estäminen.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


